
## Remote Desktop

**¿Qué es?**  
Tecnología que permite interactuar con el escritorio de un equipo remoto mediante una conexión de red, proporcionando acceso a su interfaz y recursos según los permisos disponibles.

**¿Dónde lo encuentro?**  
En sistemas Windows y entornos empresariales donde administradores o usuarios necesitan acceder remotamente a estaciones de trabajo y servidores.

**¿Por qué me afecta?**  
Una configuración insegura, credenciales comprometidas o exposición innecesaria pueden proporcionar a un atacante una vía de acceso remoto y facilitar el movimiento lateral.

**¿Cómo se soluciona?**  
Restringir el acceso mediante VPN o controles de red, utilizar autenticación robusta, limitar usuarios autorizados, aplicar MFA cuando sea posible y monitorear los inicios de sesión remotos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar credenciales comprometidas para iniciar una sesión remota y operar sobre un equipo como si fuera un usuario legítimo.


## Scheduled Task

**¿Qué es?**  
Mecanismo del sistema operativo que permite programar la ejecución automática de programas o comandos en determinados momentos o bajo condiciones específicas.

**¿Dónde lo encuentro?**  
En sistemas Windows mediante el Programador de tareas y en otros sistemas operativos mediante mecanismos equivalentes de programación de tareas.

**¿Por qué me afecta?**  
Las tareas programadas pueden utilizarse legítimamente para automatización, pero también pueden proporcionar persistencia o ejecutar acciones maliciosas de forma periódica.

**¿Cómo se soluciona?**  
Revisar periódicamente las tareas existentes, restringir permisos administrativos, monitorizar la creación o modificación de tareas y eliminar aquellas que no tengan una finalidad legítima.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de comprometer un sistema, podría crear o modificar una tarea para ejecutar automáticamente código malicioso y mantener persistencia.


## Service Execution

**¿Qué es?**  
Técnica que consiste en ejecutar código o programas mediante servicios del sistema operativo, aprovechando mecanismos legítimos de administración y ejecución.

**¿Dónde lo encuentro?**  
Principalmente en sistemas Windows y entornos empresariales donde los servicios ejecutan aplicaciones o procesos de forma automática o bajo cuentas específicas.

**¿Por qué me afecta?**  
Un atacante con los permisos adecuados puede abusar de servicios para ejecutar código, mantener persistencia o realizar movimiento lateral.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, restringir quién puede crear o modificar servicios, mantener sistemas actualizados y monitorear cambios y ejecuciones anómalas de servicios.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría crear, modificar o utilizar un servicio existente para ejecutar código bajo los privilegios asociados al servicio.


## Data Staging

**¿Qué es?**  
Técnica que consiste en recopilar y preparar información en una ubicación intermedia antes de transferirla fuera del entorno comprometido.

**¿Dónde lo encuentro?**  
En sistemas comprometidos donde un atacante reúne documentos, bases de datos, credenciales u otros archivos antes de realizar una extracción.

**¿Por qué me afecta?**  
El almacenamiento temporal de grandes cantidades de información puede indicar una fase previa a la exfiltración y aumentar el riesgo de pérdida de datos sensibles.

**¿Cómo se soluciona?**  
Monitorear accesos y movimientos inusuales de archivos, controlar permisos, detectar grandes volúmenes de datos recopilados y utilizar controles de prevención de pérdida de información cuando corresponda.

**¿Cómo lo usaría un atacante en mi contra?**  
Recopilaría información de diferentes ubicaciones y la concentraría en un directorio, sistema o recurso controlado para prepararla antes de extraerla.


## Data Exfiltration

**¿Qué es?**  
Proceso mediante el cual información obtenida de un sistema o red comprometida es transferida hacia una ubicación controlada por un atacante.

**¿Dónde lo encuentro?**  
En incidentes de robo de información, especialmente después de fases de reconocimiento, recopilación y preparación de datos.

**¿Por qué me afecta?**  
Puede provocar la exposición de información confidencial, propiedad intelectual, credenciales o datos de clientes, además de generar consecuencias legales y operativas.

**¿Cómo se soluciona?**  
Controlar las comunicaciones salientes, aplicar DLP cuando sea apropiado, limitar permisos de acceso a datos y monitorear transferencias inusuales mediante logs de red, proxy, firewall y endpoints.

**¿Cómo lo usaría un atacante en mi contra?**  
Transferiría información recopilada desde los sistemas comprometidos hacia una infraestructura bajo su control, intentando ocultar o mezclar el tráfico con comunicaciones legítimas.
