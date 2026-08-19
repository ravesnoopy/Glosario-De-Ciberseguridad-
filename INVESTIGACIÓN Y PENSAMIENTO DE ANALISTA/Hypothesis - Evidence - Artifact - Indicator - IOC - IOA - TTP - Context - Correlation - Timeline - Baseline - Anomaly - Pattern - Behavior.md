
## Hypothesis

**¿Qué es?**  
Suposición fundamentada que plantea una posible explicación para una actividad o incidente y que puede ser comprobada mediante evidencia.

**¿Dónde lo encuentro?**  
En investigaciones de incidentes, threat hunting, análisis forense y procesos de investigación de seguridad.

**¿Por qué me afecta?**  
Permite orientar la investigación sin asumir que una explicación es correcta antes de validar los datos disponibles.

**¿Cómo se soluciona?**  
Formular hipótesis verificables, contrastarlas con múltiples fuentes de evidencia y modificarlas cuando los datos no las respaldan.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar actividad que apoye una explicación falsa o distraiga a los investigadores hacia una hipótesis incorrecta.


## Evidence

**¿Qué es?**  
Información observable que puede utilizarse para demostrar, respaldar o refutar una conclusión durante una investigación de seguridad.

**¿Dónde lo encuentro?**  
En logs, sistemas de archivos, memoria, tráfico de red, registros de autenticación, alertas y otros datos obtenidos durante una investigación.

**¿Por qué me afecta?**  
La calidad y preservación de la evidencia determinan qué tan confiables son las conclusiones sobre un incidente.

**¿Cómo se soluciona?**  
Preservar la evidencia original, documentar su procedencia y analizarla junto con otras fuentes para validar los hallazgos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría eliminar, modificar o contaminar evidencias para dificultar la investigación y reducir la certeza de las conclusiones.


## Artifact

**¿Qué es?**  
Elemento o registro generado por un sistema, aplicación o usuario que puede contener información útil para una investigación.

**¿Dónde lo encuentro?**  
En sistemas operativos, discos, memoria, navegadores, registros, aplicaciones y dispositivos.

**¿Por qué me afecta?**  
Los artefactos pueden revelar acciones realizadas, programas utilizados, archivos manipulados o actividad de un usuario.

**¿Cómo se soluciona?**  
Preservarlos correctamente, identificar su origen y analizarlos en conjunto con otras fuentes para determinar su significado.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría eliminar o manipular artefactos para reducir los rastros disponibles sobre sus actividades.


## Indicator

**¿Qué es?**  
Dato observable que puede señalar una condición, actividad o comportamiento relevante para la seguridad, aunque no necesariamente confirme un compromiso.

**¿Dónde lo encuentro?**  
En logs, alertas, sistemas de monitoreo, análisis de red, endpoints y plataformas de inteligencia de amenazas.

**¿Por qué me afecta?**  
Los indicadores ayudan a identificar señales que requieren investigación y pueden servir como punto de partida para detectar amenazas.

**¿Cómo se soluciona?**  
Validar su contexto, correlacionarlos con otras señales y evitar tratarlos como evidencia definitiva sin confirmación adicional.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría evitar comportamientos que generen indicadores conocidos o modificar sus técnicas para reducir las señales detectables.


## IOC

**¿Qué es?**  
Indicator of Compromise es un artefacto o dato que puede proporcionar evidencia de que un sistema estuvo involucrado en una actividad maliciosa, como un hash, dominio, IP o archivo.

**¿Dónde lo encuentro?**  
En investigaciones forenses, inteligencia de amenazas, SIEM, EDR, logs y reportes de incidentes.

**¿Por qué me afecta?**  
Permite buscar evidencias de compromiso en otros sistemas y ampliar el alcance de una investigación.

**¿Cómo se soluciona?**  
Validar los IOC, correlacionarlos con el contexto del entorno y utilizarlos para crear o mejorar detecciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría cambiar su infraestructura o indicadores conocidos para evitar ser detectado mediante búsquedas basadas únicamente en IOC.


## IOA

**¿Qué es?**  
Indicator of Attack es una señal basada principalmente en acciones o comportamientos que pueden indicar que un ataque está ocurriendo, independientemente de un indicador específico.

**¿Dónde lo encuentro?**  
En EDR, SIEM, análisis de comportamiento, monitoreo de endpoints y sistemas de detección.

**¿Por qué me afecta?**  
Permite detectar técnicas de ataque incluso cuando el atacante cambia archivos, hashes, dominios u otros IOC.

**¿Cómo se soluciona?**  
Definir detecciones basadas en comportamientos y correlacionarlas con identidad, procesos, red y contexto del sistema.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría realizar sus acciones de forma que se parezcan a actividades legítimas o distribuirlas para reducir señales claramente sospechosas.


## TTP

**¿Qué es?**  
Tactics, Techniques and Procedures describe los objetivos, métodos y procedimientos concretos utilizados por un atacante durante una operación.

**¿Dónde lo encuentro?**  
En threat intelligence, investigaciones de incidentes, threat hunting y marcos como MITRE ATT&CK.

**¿Por qué me afecta?**  
Analizar TTP permite detectar comportamientos de ataque incluso cuando cambian las herramientas o indicadores utilizados.

**¿Cómo se soluciona?**  
Mapear comportamientos observados a técnicas conocidas y desarrollar detecciones y controles adecuados para esas actividades.

**¿Cómo lo usaría un atacante en mi contra?**  
Adaptaría sus herramientas o infraestructura mientras mantiene técnicas similares, intentando evitar las detecciones existentes.


## Context

**¿Qué es?**  
Información adicional que permite interpretar correctamente un evento o indicador considerando su entorno, momento, usuario, sistema y actividad relacionada.

**¿Dónde lo encuentro?**  
En investigaciones de seguridad, análisis de logs, alertas, threat intelligence y respuesta a incidentes.

**¿Por qué me afecta?**  
Un mismo evento puede ser normal o malicioso dependiendo del contexto, por lo que ignorarlo puede generar falsos positivos o pasar por alto amenazas.

**¿Cómo se soluciona?**  
Correlacionar eventos con usuarios, activos, horarios, procesos, ubicaciones y actividad histórica relevante.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría mezclarse con actividades legítimas para que sus acciones parezcan normales dentro del contexto operativo.


## Correlation

**¿Qué es?**  
Proceso de relacionar eventos o datos de diferentes fuentes para identificar una actividad común, una secuencia o un comportamiento relevante.

**¿Dónde lo encuentro?**  
En SIEM, SOC, análisis de logs, threat hunting e investigaciones de incidentes.

**¿Por qué me afecta?**  
La correlación permite detectar ataques que no serían evidentes al analizar cada evento de forma aislada.

**¿Cómo se soluciona?**  
Integrar fuentes relevantes, utilizar reglas de correlación y considerar tiempo, identidad, origen, destino y comportamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría distribuir sus acciones entre diferentes sistemas o identidades para dificultar que los eventos sean relacionados.


## Timeline

**¿Qué es?**  
Representación cronológica de eventos que permite reconstruir la secuencia de actividades ocurridas durante una investigación.

**¿Dónde lo encuentro?**  
En análisis forense, respuesta a incidentes, logs, sistemas de autenticación, endpoints y registros de red.

**¿Por qué me afecta?**  
Permite determinar qué ocurrió primero, relacionar eventos y reconstruir la progresión de un incidente.

**¿Cómo se soluciona?**  
Normalizar horarios, correlacionar múltiples fuentes y validar los eventos para construir una secuencia confiable.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría eliminar o manipular registros temporales para dificultar la reconstrucción de sus actividades.


## Baseline

**¿Qué es?**  
Representación del comportamiento o configuración considerada normal para un sistema, usuario, red o entorno.

**¿Dónde lo encuentro?**  
En monitoreo de seguridad, SIEM, EDR, análisis de comportamiento, gestión de configuraciones y threat hunting.

**¿Por qué me afecta?**  
Permite comparar la actividad actual con el comportamiento esperado e identificar desviaciones potencialmente sospechosas.

**¿Cómo se soluciona?**  
Definir baselines realistas, actualizarlos cuando cambie el entorno y utilizarlos junto con contexto para evitar falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría imitar comportamientos normales para evitar desviaciones suficientemente grandes como para generar alertas.


## Anomaly

**¿Qué es?**  
Actividad o condición que se desvía de un comportamiento, configuración o patrón considerado normal.

**¿Dónde lo encuentro?**  
En sistemas de monitoreo, SIEM, EDR, análisis de comportamiento, redes y registros de actividad.

**¿Por qué me afecta?**  
Una anomalía puede revelar actividad maliciosa, cuentas comprometidas, errores de configuración o comportamientos inesperados.

**¿Cómo se soluciona?**  
Analizar la anomalía dentro de su contexto, determinar su causa y establecer una respuesta cuando represente una amenaza real.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría mantener sus actividades dentro de patrones normales para reducir la probabilidad de ser identificado como una anomalía.


## Pattern

**¿Qué es?**  
Comportamiento o secuencia que se repite y puede ayudar a identificar una actividad, tendencia o técnica determinada.

**¿Dónde lo encuentro?**  
En análisis de logs, threat hunting, inteligencia de amenazas, monitoreo de usuarios y detección de incidentes.

**¿Por qué me afecta?**  
Reconocer patrones permite detectar comportamientos repetitivos que podrían indicar una campaña, técnica de ataque o actividad anómala.

**¿Cómo se soluciona?**  
Analizar múltiples eventos, identificar patrones relevantes y convertir los hallazgos en detecciones o controles cuando corresponda.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría variar sus acciones para evitar crear patrones repetitivos que faciliten su detección.


## Behavior

**¿Qué es?**  
Forma en que un usuario, proceso, sistema o entidad actúa dentro de un entorno durante un periodo determinado.

**¿Dónde lo encuentro?**  
En telemetría de endpoints, logs, redes, aplicaciones, sistemas de identidad y plataformas de análisis de comportamiento.

**¿Por qué me afecta?**  
El análisis de comportamiento permite detectar actividades sospechosas aunque no existan IOC conocidos.

**¿Cómo se soluciona?**  
Establecer comportamientos esperados, monitorear desviaciones y correlacionar las acciones con el contexto del usuario y del sistema.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría adoptar comportamientos similares a los de usuarios o procesos legítimos para mezclarse con la actividad normal del entorno.
