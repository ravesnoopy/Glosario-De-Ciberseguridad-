
## Query

**¿Qué es?**  
Consulta utilizada para buscar, recuperar o analizar información dentro de un conjunto de datos, registros o eventos.

**¿Dónde lo encuentro?**  
En SIEM, bases de datos, plataformas de monitoreo, herramientas de análisis y sistemas de búsqueda de logs.

**¿Por qué me afecta?**  
Permite localizar evidencia, investigar eventos y encontrar patrones relacionados con actividades sospechosas.

**¿Cómo se soluciona?**  
Construir consultas precisas, utilizar campos relevantes y validar los resultados para evitar conclusiones incorrectas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría realizar actividades que eviten las condiciones utilizadas por las consultas de detección o generen datos difíciles de distinguir del comportamiento legítimo.


## Filter

**¿Qué es?**  
Operación que limita los resultados de una consulta según condiciones específicas, como usuario, IP, evento, fecha o proceso.

**¿Dónde lo encuentro?**  
En SIEM, herramientas de análisis de logs, bases de datos y plataformas de monitoreo.

**¿Por qué me afecta?**  
Permite reducir grandes cantidades de eventos hasta encontrar aquellos relevantes para una investigación o detección.

**¿Cómo se soluciona?**  
Definir filtros adecuados, validar que no excluyan evidencia importante y ajustar las condiciones según el contexto.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría modificar su comportamiento para evitar los criterios utilizados por los filtros de detección.


## Aggregation

**¿Qué es?**  
Operación que agrupa o resume múltiples eventos para obtener información como conteos, frecuencias o tendencias.

**¿Dónde lo encuentro?**  
En SIEM, bases de datos, plataformas de análisis y herramientas de observabilidad.

**¿Por qué me afecta?**  
Permite identificar patrones que no serían evidentes al analizar eventos individualmente, como numerosos intentos de autenticación.

**¿Cómo se soluciona?**  
Agrupar eventos mediante campos relevantes y establecer umbrales basados en el comportamiento normal del entorno.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría distribuir sus acciones o reducir su frecuencia para mantenerse por debajo de determinados umbrales de detección.


## Field Extraction

**¿Qué es?**  
Proceso de identificar y separar datos específicos dentro de un evento para convertirlos en campos analizables.

**¿Dónde lo encuentro?**  
En SIEM, pipelines de procesamiento de logs, herramientas de análisis y sistemas de ingestión de datos.

**¿Por qué me afecta?**  
Una extracción incorrecta puede impedir búsquedas, correlaciones y detecciones sobre información importante.

**¿Cómo se soluciona?**  
Definir correctamente los campos, validar los formatos de los logs y comprobar que la extracción funcione con diferentes eventos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar datos con formatos inesperados para dificultar su extracción, normalización o posterior detección.


## Regex

**¿Qué es?**  
Expresión regular utilizada para buscar, identificar o extraer patrones específicos dentro de texto o datos.

**¿Dónde lo encuentro?**  
En SIEM, herramientas de análisis, lenguajes de programación, procesamiento de logs y sistemas de detección.

**¿Por qué me afecta?**  
Permite identificar patrones como nombres de archivos, direcciones IP, comandos o cadenas sospechosas dentro de grandes volúmenes de información.

**¿Cómo se soluciona?**  
Diseñar expresiones precisas, probarlas con datos reales y evitar patrones demasiado amplios o costosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría modificar la representación de una entrada maliciosa para evitar que coincida con patrones de detección demasiado específicos.


## KQL

**¿Qué es?**  
Kusto Query Language es un lenguaje utilizado para consultar y analizar grandes volúmenes de datos, especialmente en plataformas de Microsoft orientadas a seguridad y observabilidad.

**¿Dónde lo encuentro?**  
En herramientas como Microsoft Sentinel y Microsoft Defender para realizar búsquedas, investigaciones y detecciones.

**¿Por qué me afecta?**  
Permite analizar eventos y construir consultas para identificar comportamientos sospechosos dentro de grandes cantidades de telemetría.

**¿Cómo se soluciona?**  
Crear consultas eficientes, utilizar campos relevantes y validar los resultados con el contexto de la organización.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría realizar actividades que eviten las condiciones de las consultas KQL utilizadas por las detecciones.


## SPL

**¿Qué es?**  
Search Processing Language es el lenguaje de búsqueda utilizado por Splunk para consultar, transformar y analizar datos de eventos.

**¿Dónde lo encuentro?**  
En Splunk, especialmente en investigaciones de SOC, análisis de logs, Threat Hunting y creación de detecciones.

**¿Por qué me afecta?**  
Permite buscar eventos, correlacionar información y construir consultas para identificar actividad sospechosa.

**¿Cómo se soluciona?**  
Diseñar búsquedas eficientes, utilizar campos normalizados y validar las detecciones con datos reales.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría modificar sus acciones para evitar las condiciones de las búsquedas y reglas basadas en SPL.


## Sigma Rule

**¿Qué es?**  
Regla de detección en formato abierto y estructurado diseñada para describir patrones de actividad sospechosa de forma independiente de un SIEM específico.

**¿Dónde lo encuentro?**  
En repositorios de detecciones, Threat Hunting, Detection Engineering y herramientas que convierten reglas Sigma a formatos compatibles con diferentes plataformas.

**¿Por qué me afecta?**  
Permite compartir y reutilizar detecciones entre diferentes tecnologías de seguridad sin depender de un lenguaje específico de un producto.

**¿Cómo se soluciona?**  
Mantener las reglas actualizadas, probarlas contra telemetría real y adaptar correctamente sus campos al entorno donde serán utilizadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría modificar su comportamiento para evitar las condiciones definidas por una regla Sigma o generar actividad similar a la legítima.


## Detection Query

**¿Qué es?**  
Consulta diseñada específicamente para identificar eventos o comportamientos que pueden indicar una amenaza o actividad maliciosa.

**¿Dónde lo encuentro?**  
En SIEM, EDR, plataformas de Threat Hunting y sistemas de Detection Engineering.

**¿Por qué me afecta?**  
Es uno de los mecanismos utilizados para transformar datos de seguridad en alertas investigables dentro de un SOC.

**¿Cómo se soluciona?**  
Diseñar consultas basadas en comportamientos relevantes, probarlas, reducir falsos positivos y mantenerlas según cambien las amenazas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría evadir las condiciones de la consulta mediante cambios en herramientas, parámetros, cuentas, tiempos o comportamientos utilizados durante el ataque.
