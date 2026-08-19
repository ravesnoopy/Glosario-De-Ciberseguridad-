
## HTTP Request

**¿Qué es?**  
Mensaje enviado por un cliente a un servidor HTTP para solicitar un recurso o realizar una acción.

**¿Dónde lo encuentro?**  
En navegadores, aplicaciones web, APIs, servidores web, proxies y registros HTTP.

**¿Por qué me afecta?**  
Permite analizar qué recursos se solicitan, desde dónde y con qué parámetros, proporcionando evidencia útil para detectar ataques web.

**¿Cómo se soluciona?**  
Validar solicitudes, autenticar correctamente, registrar eventos relevantes y proteger las aplicaciones contra entradas maliciosas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría enviar solicitudes manipuladas para explotar vulnerabilidades, obtener información o ejecutar acciones no autorizadas.


## HTTP Response

**¿Qué es?**  
Mensaje que un servidor HTTP devuelve como respuesta a una solicitud realizada por un cliente.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, navegadores, proxies y registros de servidores web.

**¿Por qué me afecta?**  
Las respuestas pueden revelar errores, información sensible o comportamientos que ayuden a identificar una intrusión.

**¿Cómo se soluciona?**  
Evitar exponer información innecesaria, configurar correctamente los servidores y registrar respuestas relevantes para investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría analizar las respuestas para descubrir tecnologías, errores, recursos existentes o información útil para continuar un ataque.


## Status Code

**¿Qué es?**  
Código numérico incluido en una respuesta HTTP que indica el resultado de una solicitud, como éxito, redirección o error.

**¿Dónde lo encuentro?**  
En respuestas HTTP, logs de servidores, proxies, navegadores y herramientas de monitoreo web.

**¿Por qué me afecta?**  
Patrones anómalos de códigos de estado pueden revelar errores, escaneos, intentos de acceso no autorizado o explotación.

**¿Cómo se soluciona?**  
Monitorear patrones de respuestas, investigar códigos anómalos y configurar correctamente las aplicaciones para no revelar información innecesaria.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría analizar códigos de estado para determinar qué recursos existen, qué solicitudes son aceptadas y cómo responde una aplicación ante entradas específicas.


## Authentication Event

**¿Qué es?**  
Evento que registra un intento o resultado relacionado con la autenticación de una identidad en un sistema o servicio.

**¿Dónde lo encuentro?**  
En Active Directory, sistemas operativos, aplicaciones, VPN, servicios cloud, IAM y sistemas SIEM.

**¿Por qué me afecta?**  
Permite detectar inicios de sesión sospechosos, intentos fallidos, uso de credenciales comprometidas y posibles movimientos laterales.

**¿Cómo se soluciona?**  
Monitorear eventos de autenticación, aplicar MFA, mínimo privilegio y políticas adecuadas de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar credenciales robadas para autenticarse y acceder a sistemas o recursos con los permisos de la cuenta comprometida.


## Network Event

**¿Qué es?**  
Evento que registra una actividad relacionada con comunicaciones de red, como conexiones, tráfico o cambios relevantes en la conectividad.

**¿Dónde lo encuentro?**  
En firewalls, routers, IDS/IPS, EDR, servidores, sistemas operativos y plataformas SIEM.

**¿Por qué me afecta?**  
Permite identificar conexiones inesperadas, escaneos, comunicaciones con infraestructura maliciosa y posibles movimientos laterales.

**¿Cómo se soluciona?**  
Centralizar y monitorear eventos de red, aplicar segmentación y establecer detecciones para comportamientos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar conexiones para explorar sistemas, comunicarse con C2 o desplazarse hacia otros recursos de la red.


## Process Event

**¿Qué es?**  
Evento que registra la creación, ejecución o finalización de un proceso en un sistema.

**¿Dónde lo encuentro?**  
En sistemas operativos, EDR, Sysmon, logs de seguridad y herramientas de monitoreo de endpoints.

**¿Por qué me afecta?**  
Los procesos proporcionan evidencia sobre qué programas se ejecutaron y qué actividad pudo realizar un atacante.

**¿Cómo se soluciona?**  
Registrar procesos relevantes, analizar relaciones padre-hijo y crear detecciones para ejecuciones anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría ejecutar procesos maliciosos o utilizar procesos legítimos para realizar acciones y dificultar su detección.


## File Event

**¿Qué es?**  
Evento relacionado con la creación, modificación, eliminación o acceso a un archivo.

**¿Dónde lo encuentro?**  
En sistemas operativos, EDR, Sysmon, servidores de archivos y herramientas de auditoría.

**¿Por qué me afecta?**  
Los cambios en archivos pueden proporcionar evidencia de malware, persistencia, manipulación de información o exfiltración.

**¿Cómo se soluciona?**  
Monitorear archivos críticos, aplicar controles de acceso y registrar modificaciones relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría crear archivos maliciosos, modificar archivos legítimos o eliminar evidencia de sus actividades.


## Registry Event

**¿Qué es?**  
Evento que registra operaciones relevantes sobre el Registro de Windows, como creación, modificación o eliminación de claves y valores.

**¿Dónde lo encuentro?**  
En Windows, Sysmon, EDR y herramientas de auditoría y monitoreo.

**¿Por qué me afecta?**  
Cambios en el registro pueden indicar persistencia, modificación de configuraciones o actividad maliciosa.

**¿Cómo se soluciona?**  
Monitorear claves sensibles, restringir privilegios y generar alertas para modificaciones inesperadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría modificar determinadas claves para establecer persistencia, alterar configuraciones o ejecutar acciones maliciosas.


## Service Event

**¿Qué es?**  
Evento relacionado con la creación, modificación, inicio, detención o eliminación de un servicio del sistema.

**¿Dónde lo encuentro?**  
En Windows, Linux, registros del sistema, EDR y herramientas de administración.

**¿Por qué me afecta?**  
Los servicios pueden proporcionar persistencia o ejecutar código con privilegios elevados.

**¿Cómo se soluciona?**  
Controlar la creación y modificación de servicios, aplicar mínimo privilegio y monitorear cambios inesperados.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría crear o modificar un servicio para ejecutar malware automáticamente o mantener persistencia.


## Scheduled Task Event

**¿Qué es?**  
Evento relacionado con la creación, modificación, ejecución o eliminación de una tarea programada.

**¿Dónde lo encuentro?**  
Principalmente en Windows, Task Scheduler, registros de eventos, Sysmon y EDR.

**¿Por qué me afecta?**  
Las tareas programadas pueden utilizarse para ejecutar acciones automáticamente y mantener persistencia.

**¿Cómo se soluciona?**  
Monitorear cambios en tareas programadas, restringir privilegios y revisar tareas desconocidas o inesperadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría crear una tarea programada para ejecutar malware periódicamente o iniciar código malicioso bajo determinadas condiciones.


## PowerShell Event

**¿Qué es?**  
Evento generado por la ejecución o actividad de PowerShell, proporcionando información sobre comandos, procesos o sesiones según la auditoría configurada.

**¿Dónde lo encuentro?**  
En registros de Windows, PowerShell, Sysmon, EDR y sistemas SIEM.

**¿Por qué me afecta?**  
PowerShell es una herramienta legítima pero puede ser utilizada para ejecutar acciones maliciosas sin necesidad de introducir herramientas adicionales.

**¿Cómo se soluciona?**  
Habilitar auditoría adecuada, monitorear comportamientos sospechosos, aplicar controles de ejecución y limitar privilegios.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar PowerShell para ejecutar código, recopilar información, descargar contenido o realizar acciones posteriores al compromiso.


## Sysmon Event

**¿Qué es?**  
Evento generado por Sysmon para registrar actividad detallada del sistema, como procesos, conexiones de red, archivos, registro y otras acciones configuradas.

**¿Dónde lo encuentro?**  
En Windows, específicamente en los registros operativos de Sysmon, y normalmente centralizado en SIEM o plataformas de monitoreo.

**¿Por qué me afecta?**  
Proporciona telemetría detallada que ayuda a investigar incidentes, correlacionar comportamientos y detectar actividad maliciosa.

**¿Cómo se soluciona?**  
Configurar Sysmon según las necesidades del entorno, centralizar sus eventos y crear detecciones sobre la telemetría relevante.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría ejecutar acciones que reduzcan su visibilidad, evadir las condiciones de detección o aprovechar comportamientos legítimos para ocultar actividad maliciosa.
