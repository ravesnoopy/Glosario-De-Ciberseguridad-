
## Severity

**¿Qué es?**  
Severity es el nivel de gravedad asignado a una alerta, evento o incidente según su impacto potencial, alcance y riesgo para la organización.

**¿Dónde lo encuentro?**  
En SIEM, EDR, sistemas de ticketing, plataformas SOC y procedimientos de respuesta a incidentes.

**¿Por qué me afecta?**  
Permite determinar qué eventos requieren atención inmediata y ayuda a asignar recursos de acuerdo con el riesgo.

**¿Cómo se soluciona?**  
Definiendo criterios consistentes de severidad basados en impacto, criticidad de los activos, alcance y evidencia disponible.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede mantener inicialmente sus actividades en un nivel de bajo impacto para evitar que sean clasificadas como incidentes de alta severidad.

## Priority

**¿Qué es?**  
Priority es el nivel de urgencia asignado a una alerta, tarea o incidente para determinar qué debe atenderse primero.

**¿Dónde lo encuentro?**  
En SOC, sistemas de ticketing, SIEM, plataformas de Incident Response y herramientas de gestión de alertas.

**¿Por qué me afecta?**  
Una prioridad incorrecta puede retrasar la atención de una amenaza crítica o hacer que recursos se dediquen a eventos menos importantes.

**¿Cómo se soluciona?**  
Estableciendo criterios de priorización basados en severidad, impacto, criticidad del activo y contexto del incidente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar actividad de bajo impacto o ruido para reducir la prioridad aparente de sus acciones reales.

## Evidence

**¿Qué es?**  
Evidence es cualquier información obtenida durante una investigación que ayuda a demostrar, comprender o reconstruir una actividad de seguridad.

**¿Dónde lo encuentro?**  
En logs, imágenes de disco, memoria, archivos, capturas de red, registros de autenticación y sistemas afectados.

**¿Por qué me afecta?**  
La evidencia permite determinar qué ocurrió, cómo ocurrió y qué sistemas o datos pudieron verse afectados.

**¿Cómo se soluciona?**  
Recolectándola de forma adecuada, preservando su integridad y documentando cómo fue obtenida y analizada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar eliminar, modificar o destruir evidencia para dificultar la investigación y ocultar sus actividades.

## Artifact

**¿Qué es?**  
Artifact es cualquier objeto, registro o dato residual dejado por una actividad realizada en un sistema y que puede aportar información durante una investigación.

**¿Dónde lo encuentro?**  
En sistemas de archivos, registros, memoria, navegadores, registros de eventos, configuración del sistema y dispositivos de almacenamiento.

**¿Por qué me afecta?**  
Los artifacts pueden revelar acciones realizadas por usuarios o atacantes incluso cuando la actividad original ya terminó.

**¿Cómo se soluciona?**  
Identificando los artifacts relevantes, recolectándolos correctamente y preservándolos para su análisis forense.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentará eliminar o modificar artifacts para reducir las evidencias que puedan vincularlo con sus acciones.

## IOC

**¿Qué es?**  
IOC (Indicator of Compromise) es un indicador técnico que puede asociarse con una posible intrusión, como una dirección IP, dominio, hash o archivo malicioso.

**¿Dónde lo encuentro?**  
En logs, EDR, SIEM, análisis de malware, threat intelligence e investigaciones forenses.

**¿Por qué me afecta?**  
Permite buscar evidencia de compromiso en sistemas y detectar infraestructura o artefactos asociados con amenazas conocidas.

**¿Cómo se soluciona?**  
Monitoreando IOCs relevantes, correlacionándolos con otras evidencias y actualizando las fuentes de inteligencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cambiar dominios, direcciones IP, hashes u otros indicadores para evitar detecciones basadas en IOCs conocidos.

## IOA

**¿Qué es?**  
IOA (Indicator of Attack) es una señal basada en el comportamiento o acciones que pueden indicar que un ataque está ocurriendo, independientemente de un indicador específico.

**¿Dónde lo encuentro?**  
En EDR, SIEM, Threat Hunting, sistemas de detección de comportamiento y plataformas de seguridad.

**¿Por qué me afecta?**  
Permite detectar comportamientos asociados con ataques incluso cuando los IOCs cambian o no son conocidos previamente.

**¿Cómo se soluciona?**  
Desarrollando detecciones basadas en comportamiento y correlacionando múltiples eventos para identificar patrones de ataque.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar utilizar técnicas legítimas del sistema y reducir o modificar sus comportamientos para evitar patrones de ataque conocidos.

## TTP

**¿Qué es?**  
TTP (Tactics, Techniques and Procedures) describe los objetivos, métodos y procedimientos utilizados por un adversario durante una operación.

**¿Dónde lo encuentro?**  
En Threat Intelligence, Threat Hunting, análisis de incidentes y marcos como MITRE ATT&CK.

**¿Por qué me afecta?**  
Comprender los TTP permite detectar comportamientos de los atacantes incluso cuando cambian herramientas o indicadores específicos.

**¿Cómo se soluciona?**  
Mapeando comportamientos observados a TTP conocidos y desarrollando detecciones y controles para las técnicas relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cambiar herramientas o infraestructura manteniendo las mismas técnicas y procedimientos para intentar conservar su capacidad operativa mientras evade detecciones específicas.

## Timeline

**¿Qué es?**  
Timeline es una representación cronológica de eventos que permite reconstruir la secuencia de actividades durante una investigación.

**¿Dónde lo encuentro?**  
En investigaciones DFIR, análisis de incidentes, SIEM, herramientas forenses y reportes de seguridad.

**¿Por qué me afecta?**  
Ayuda a determinar cuándo comenzó una actividad, qué ocurrió después y cómo evolucionó un incidente.

**¿Cómo se soluciona?**  
Correlacionando timestamps de múltiples fuentes, verificando zonas horarias y organizando los eventos en orden cronológico.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar timestamps, eliminar registros o realizar acciones espaciadas para dificultar la reconstrucción de la línea temporal.

## Event ID

**¿Qué es?**  
Event ID es un identificador utilizado para distinguir un tipo específico de evento registrado por un sistema o aplicación.

**¿Dónde lo encuentro?**  
En Windows Event Log, aplicaciones, SIEM y otras plataformas que recopilan eventos.

**¿Por qué me afecta?**  
Permite identificar rápidamente determinados eventos y facilita la creación de filtros y reglas de detección.

**¿Cómo se soluciona?**  
Conociendo los Event ID relevantes para el entorno y correlacionándolos con otros campos y fuentes de información.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar actividad que produzca eventos similares a los legítimos o intentar evitar que determinados eventos sean registrados.

## Logon Type

**¿Qué es?**  
Logon Type es un valor que indica la forma en que una cuenta inició sesión o se autenticó en un sistema Windows.

**¿Dónde lo encuentro?**  
En eventos de seguridad de Windows, especialmente en registros relacionados con autenticaciones y cuentas.

**¿Por qué me afecta?**  
Permite distinguir diferentes formas de acceso y detectar patrones sospechosos, como autenticaciones remotas inesperadas o uso anómalo de cuentas.

**¿Cómo se soluciona?**  
Monitoreando los tipos de inicio de sesión relevantes, correlacionándolos con usuarios, equipos, horarios y origen de la conexión.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas mediante métodos de acceso legítimos, como autenticaciones remotas, para mezclarse con la actividad normal del entorno.
