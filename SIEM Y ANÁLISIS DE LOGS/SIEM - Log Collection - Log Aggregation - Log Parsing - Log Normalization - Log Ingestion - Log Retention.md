
## SIEM

**¿Qué es?**  
SIEM (Security Information and Event Management) es una plataforma que centraliza, analiza y correlaciona eventos de seguridad provenientes de diferentes fuentes.

**¿Dónde lo encuentro?**  
En centros de operaciones de seguridad (SOC), entornos empresariales y plataformas de monitoreo que integran logs de endpoints, servidores, redes y aplicaciones.

**¿Por qué me afecta?**  
Permite detectar actividades sospechosas, correlacionar eventos y generar alertas que ayudan a investigar incidentes de seguridad.

**¿Cómo se soluciona?**  
Configurando correctamente las fuentes de logs, reglas de correlación, alertas, retención y controles de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evadir las reglas de detección, generar ruido para ocultar actividades maliciosas o atacar las fuentes de logs para reducir la visibilidad.

## Log Collection

**¿Qué es?**  
Log Collection es el proceso de recopilar registros generados por diferentes sistemas, aplicaciones y dispositivos.

**¿Dónde lo encuentro?**  
En SIEM, servidores de logging, agentes instalados en endpoints, dispositivos de red y plataformas de monitoreo.

**¿Por qué me afecta?**  
Sin una recopilación adecuada, eventos importantes pueden quedar fuera de la visibilidad del equipo de seguridad.

**¿Cómo se soluciona?**  
Identificando fuentes críticas, configurando agentes o mecanismos de recolección y verificando continuamente que los logs lleguen correctamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer una fuente de logs o interrumpir su envío para evitar que sus actividades sean registradas y analizadas.

## Log Aggregation

**¿Qué es?**  
Log Aggregation es el proceso de reunir registros provenientes de múltiples fuentes en un sistema o ubicación centralizada.

**¿Dónde lo encuentro?**  
En SIEM, servidores de logs, plataformas de observabilidad y arquitecturas centralizadas de monitoreo.

**¿Por qué me afecta?**  
Facilita la correlación de eventos de diferentes sistemas y permite obtener una visión más completa de una actividad.

**¿Cómo se soluciona?**  
Centralizando las fuentes relevantes, manteniendo una infraestructura de almacenamiento adecuada y verificando la integridad de los registros.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar grandes cantidades de eventos para producir ruido y dificultar que los analistas identifiquen señales relevantes.

## Log Parsing

**¿Qué es?**  
Log Parsing es el proceso de interpretar un registro y separar su contenido en campos estructurados para facilitar su análisis.

**¿Dónde lo encuentro?**  
En SIEM, pipelines de procesamiento de logs, herramientas de análisis y sistemas de monitoreo.

**¿Por qué me afecta?**  
Un parsing incorrecto puede provocar que información importante no sea interpretada correctamente y afectar las detecciones.

**¿Cómo se soluciona?**  
Validando los parsers, adaptándolos al formato real de los logs y verificando periódicamente que los campos se procesen correctamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar entradas especialmente diseñadas para confundir el procesamiento de logs o provocar que determinados eventos sean interpretados incorrectamente.

## Log Normalization

**¿Qué es?**  
Log Normalization es el proceso de convertir registros de diferentes fuentes a una estructura y formato común para facilitar su comparación y correlación.

**¿Dónde lo encuentro?**  
En SIEM, pipelines de ingestión, plataformas de análisis y sistemas que integran múltiples fuentes de seguridad.

**¿Por qué me afecta?**  
Permite correlacionar eventos que utilizan formatos diferentes y mejora la consistencia de las reglas de detección.

**¿Cómo se soluciona?**  
Definiendo esquemas consistentes, validando los campos normalizados y manteniendo actualizados los procesos de transformación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar diferencias o errores en la normalización para generar eventos que no sean interpretados correctamente por las detecciones.

## Log Ingestion

**¿Qué es?**  
Log Ingestion es el proceso mediante el cual una plataforma recibe e incorpora registros provenientes de diferentes fuentes para su posterior procesamiento y análisis.

**¿Dónde lo encuentro?**  
En SIEM, plataformas de logging, pipelines de datos y sistemas centralizados de monitoreo.

**¿Por qué me afecta?**  
Una ingestión incompleta, retrasada o incorrecta puede provocar pérdida de visibilidad sobre actividades relevantes para la seguridad.

**¿Cómo se soluciona?**  
Monitoreando el flujo de datos, validando formatos, controlando errores y verificando que las fuentes críticas estén enviando eventos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar interrumpir o saturar el proceso de ingestión para provocar pérdida de eventos o retrasar su análisis.

## Log Retention

**¿Qué es?**  
Log Retention es el período durante el cual los registros se conservan antes de ser eliminados o archivados.

**¿Dónde lo encuentro?**  
En SIEM, servidores de logs, sistemas de almacenamiento, plataformas cloud y políticas de gestión de registros.

**¿Por qué me afecta?**  
Una retención insuficiente puede eliminar evidencia necesaria para investigar incidentes que fueron descubiertos días o semanas después.

**¿Cómo se soluciona?**  
Definiendo períodos de retención según necesidades operativas, legales y de seguridad, además de proteger los registros contra modificaciones o eliminación no autorizada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar registros o permanecer inactivo durante suficiente tiempo para que la evidencia de sus primeras actividades sea eliminada por las políticas de retención.
