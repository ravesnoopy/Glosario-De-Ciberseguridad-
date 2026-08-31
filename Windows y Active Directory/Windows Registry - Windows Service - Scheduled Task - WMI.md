# Windows Registry

**¿Qué es?**  
Windows Registry es una base de datos jerárquica utilizada por Windows para almacenar configuraciones del sistema operativo, aplicaciones, usuarios y componentes.

**¿Dónde lo encuentro?**  
En sistemas Windows, donde puede consultarse y administrarse mediante herramientas como Registry Editor (`regedit`) y diferentes mecanismos de administración.

**¿Por qué me afecta?**  
El Registry contiene configuraciones importantes del sistema y aplicaciones. Cambios no autorizados pueden modificar comportamientos, debilitar controles de seguridad o establecer mecanismos de persistencia.

**¿Cómo se soluciona?**  
Restringiendo los permisos de modificación, monitoreando cambios en claves sensibles y aplicando configuraciones de seguridad estandarizadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar determinadas claves y valores para alterar configuraciones, ejecutar componentes automáticamente o establecer persistencia.

---

# Windows Service

**¿Qué es?**  
Windows Service es un componente que puede ejecutarse en segundo plano y realizar tareas de forma continua o bajo determinadas condiciones sin requerir una interacción directa del usuario.

**¿Dónde lo encuentro?**  
En sistemas Windows, especialmente en servidores y equipos que ejecutan aplicaciones o componentes que funcionan como servicios.

**¿Por qué me afecta?**  
Los servicios pueden ejecutarse con privilegios elevados y tener acceso a recursos importantes del sistema.

**¿Cómo se soluciona?**  
Revisando los servicios instalados, deshabilitando los innecesarios, aplicando mínimo privilegio y monitoreando modificaciones en su configuración.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar modificar un servicio existente o crear uno nuevo para ejecutar código con determinados privilegios y mantener persistencia.

---

# Scheduled Task

**¿Qué es?**  
Scheduled Task es una tarea configurada en Windows para ejecutar automáticamente un programa, script o comando cuando se cumple un horario o condición determinada.

**¿Dónde lo encuentro?**  
En Windows mediante Task Scheduler (`taskschd.msc`) y en registros asociados con la creación, modificación y ejecución de tareas.

**¿Por qué me afecta?**  
Las tareas programadas son una función legítima de automatización, pero una tarea no autorizada puede utilizarse para ejecutar código automáticamente o mantener persistencia.

**¿Cómo se soluciona?**  
Revisando las tareas existentes, eliminando las no autorizadas y monitoreando su creación, modificación y ejecución.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede crear o modificar una tarea para ejecutar un programa o script de forma periódica o durante determinados eventos.

---

# WMI

**¿Qué es?**  
WMI (Windows Management Instrumentation) es una tecnología de Windows que proporciona una interfaz para consultar y administrar información y componentes del sistema.

**¿Dónde lo encuentro?**  
En sistemas Windows, herramientas administrativas, scripts, aplicaciones y soluciones de gestión empresarial.

**¿Por qué me afecta?**  
WMI proporciona capacidades administrativas legítimas que pueden ser utilizadas para consultar sistemas, interactuar con procesos y realizar tareas de administración.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, restringiendo quién puede utilizar WMI, monitoreando actividades administrativas y registrando operaciones relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede abusar de WMI para recopilar información, ejecutar acciones o interactuar con otros sistemas después de obtener los permisos necesarios.
