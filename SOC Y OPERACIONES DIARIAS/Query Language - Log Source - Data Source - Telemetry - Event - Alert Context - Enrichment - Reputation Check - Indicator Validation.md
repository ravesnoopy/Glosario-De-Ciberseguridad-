
## Query Language

**¿Qué es?**  
Lenguaje utilizado para consultar, filtrar y analizar datos almacenados en plataformas como SIEM, bases de datos o sistemas de monitoreo.

**¿Dónde lo encuentro?**  
En SIEM, herramientas de Threat Hunting, plataformas de observabilidad y sistemas de análisis de datos.

**¿Por qué me afecta?**  
Permite investigar eventos, buscar indicadores y construir consultas para detectar comportamientos sospechosos.

**¿Cómo se soluciona?**  
Utilizar correctamente la sintaxis del lenguaje, validar los resultados y mantener las consultas adaptadas a los datos disponibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría realizar actividades que no coincidan con los patrones utilizados por las consultas de detección.


## Log Source

**¿Qué es?**  
Sistema, aplicación o dispositivo que genera registros de actividad y los proporciona para su análisis.

**¿Dónde lo encuentro?**  
En servidores, endpoints, firewalls, aplicaciones, sistemas cloud, dispositivos de red y servicios de autenticación.

**¿Por qué me afecta?**  
Una fuente de logs incompleta o mal configurada puede dejar actividades importantes fuera de la visibilidad del SOC.

**¿Cómo se soluciona?**  
Identificar las fuentes críticas, configurar correctamente la generación y centralización de logs y verificar su disponibilidad.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría dirigirse hacia sistemas con poca o ninguna generación de logs para reducir la visibilidad de sus acciones.


## Data Source

**¿Qué es?**  
Origen del que se obtiene información utilizada para monitoreo, análisis, detección o investigación de seguridad.

**¿Dónde lo encuentro?**  
En SIEM, EDR, firewalls, sistemas operativos, aplicaciones, servicios cloud y otras plataformas de seguridad.

**¿Por qué me afecta?**  
La calidad y cobertura de las fuentes de datos determinan qué actividades puede observar y detectar un SOC.

**¿Cómo se soluciona?**  
Definir las fuentes necesarias según los riesgos del entorno, centralizar los datos relevantes y verificar su calidad.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría operar en áreas con poca cobertura de datos para dificultar la detección y reconstrucción de sus acciones.


## Telemetry

**¿Qué es?**  
Datos generados por sistemas, dispositivos y aplicaciones que describen su actividad y comportamiento.

**¿Dónde lo encuentro?**  
En EDR, SIEM, sistemas operativos, aplicaciones, redes, servicios cloud y herramientas de monitoreo.

**¿Por qué me afecta?**  
La telemetría proporciona visibilidad necesaria para detectar, investigar y responder ante comportamientos anómalos.

**¿Cómo se soluciona?**  
Recopilar telemetría relevante, protegerla, centralizarla y garantizar que tenga suficiente calidad y contexto.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría reducir, evadir o mezclarse con la telemetría legítima para dificultar la identificación de sus actividades.


## Event

**¿Qué es?**  
Registro de una acción, cambio o actividad que ocurre dentro de un sistema, aplicación, red o servicio.

**¿Dónde lo encuentro?**  
En logs de sistemas operativos, aplicaciones, dispositivos de red, EDR, SIEM y servicios cloud.

**¿Por qué me afecta?**  
Los eventos constituyen la evidencia básica utilizada para investigar incidentes y detectar comportamientos sospechosos.

**¿Cómo se soluciona?**  
Registrar eventos relevantes, conservarlos correctamente y correlacionarlos con otras fuentes de información.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría generar eventos similares a actividades legítimas o eliminar y alterar registros cuando tenga capacidad para hacerlo.


## Alert Context

**¿Qué es?**  
Información adicional asociada a una alerta que ayuda al analista a comprender su origen, alcance, riesgo y posible significado.

**¿Dónde lo encuentro?**  
En SIEM, EDR, plataformas de detección, sistemas de tickets y herramientas de gestión de incidentes.

**¿Por qué me afecta?**  
Un contexto insuficiente puede provocar que una alerta importante sea interpretada incorrectamente o investigada con retraso.

**¿Cómo se soluciona?**  
Incluir datos como usuario, host, IP, proceso, tiempo, eventos relacionados y otros elementos relevantes para la investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría generar actividad ambigua o distribuida para dificultar que una alerta individual proporcione suficiente contexto.


## Enrichment

**¿Qué es?**  
Proceso de añadir información adicional a un evento o indicador para mejorar su análisis y contexto.

**¿Dónde lo encuentro?**  
En SIEM, SOAR, plataformas de Threat Intelligence, EDR y flujos de investigación de SOC.

**¿Por qué me afecta?**  
Permite complementar una alerta con información como reputación, geolocalización, identidad, historial o inteligencia de amenazas.

**¿Cómo se soluciona?**  
Integrar fuentes confiables, validar la información obtenida y evitar depender de una única fuente de enriquecimiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar infraestructura nueva o poco conocida que todavía no tenga suficiente información de reputación o inteligencia asociada.


## Reputation Check

**¿Qué es?**  
Proceso de consultar fuentes de reputación para determinar si un indicador, como una IP, dominio, archivo o URL, está asociado con actividad maliciosa conocida.

**¿Dónde lo encuentro?**  
En SIEM, EDR, plataformas de Threat Intelligence y herramientas de análisis de indicadores.

**¿Por qué me afecta?**  
Ayuda a priorizar investigaciones y determinar si un indicador tiene antecedentes relacionados con amenazas conocidas.

**¿Cómo se soluciona?**  
Consultar múltiples fuentes confiables y considerar la antigüedad, contexto y confiabilidad de la reputación obtenida.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar infraestructura nueva, comprometida o con poca reputación conocida para reducir la probabilidad de ser identificado mediante consultas de reputación.


## Indicator Validation

**¿Qué es?**  
Proceso de comprobar si un indicador de compromiso es válido, relevante y realmente está relacionado con actividad sospechosa.

**¿Dónde lo encuentro?**  
En Threat Intelligence, SOC, Threat Hunting, análisis de malware y respuesta a incidentes.

**¿Por qué me afecta?**  
Evita generar conclusiones incorrectas a partir de indicadores obsoletos, falsos positivos o información sin suficiente contexto.

**¿Cómo se soluciona?**  
Correlacionar el indicador con otras evidencias, verificar su origen y analizarlo dentro del contexto del entorno afectado.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría reutilizar indicadores compartidos o conocidos dentro de actividad legítima para generar confusión y dificultar la validación de los verdaderos indicadores.
