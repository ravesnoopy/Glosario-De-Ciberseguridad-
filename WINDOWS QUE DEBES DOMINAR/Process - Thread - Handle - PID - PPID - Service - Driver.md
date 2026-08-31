# Process

**¿Qué es?**  
Process es una instancia en ejecución de un programa que contiene el código, memoria y recursos necesarios para realizar una tarea dentro de un sistema operativo.

**¿Dónde lo encuentro?**  
En sistemas operativos, administradores de tareas, herramientas de monitoreo, EDR y registros de actividad.

**¿Por qué me afecta?**  
Los procesos permiten identificar qué programas están ejecutándose y pueden revelar actividad anómala o maliciosa durante una investigación.

**¿Cómo se soluciona?**  
Monitoreando procesos, analizando su origen, línea de comandos, usuario, proceso padre y comportamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede ejecutar procesos maliciosos o abusar de procesos legítimos para realizar actividades sin llamar demasiado la atención.

---

# Thread

**¿Qué es?**  
Thread es una unidad de ejecución dentro de un proceso que permite realizar tareas de manera independiente o concurrente.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, herramientas de análisis de procesos y soluciones EDR.

**¿Por qué me afecta?**  
El análisis de threads puede revelar actividad que no es evidente únicamente observando el proceso principal.

**¿Cómo se soluciona?**  
Monitoreando comportamientos anómalos, creación de threads y relaciones entre procesos cuando sea relevante para la investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar threads dentro de procesos legítimos para ejecutar código o realizar actividades maliciosas sin crear necesariamente un proceso independiente.

---

# Handle

**¿Qué es?**  
Handle es una referencia utilizada por un proceso para acceder a un recurso administrado por el sistema operativo, como archivos, procesos, claves de registro o eventos.

**¿Dónde lo encuentro?**  
En sistemas operativos Windows y herramientas de análisis y diagnóstico de procesos.

**¿Por qué me afecta?**  
Los handles permiten conocer qué recursos está utilizando un proceso y pueden proporcionar contexto durante una investigación.

**¿Cómo se soluciona?**  
Monitoreando accesos inusuales a recursos y analizando los handles cuando exista actividad sospechosa.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener acceso a recursos mediante procesos que ya tengan permisos sobre ellos.

---

# PID

**¿Qué es?**  
PID (Process ID) es un identificador numérico asignado por el sistema operativo a un proceso en ejecución.

**¿Dónde lo encuentro?**  
En Task Manager, herramientas de línea de comandos, EDR, registros y herramientas de administración del sistema.

**¿Por qué me afecta?**  
Permite identificar y correlacionar un proceso específico entre diferentes herramientas y eventos.

**¿Cómo se soluciona?**  
Utilizando el PID junto con otros datos como nombre del proceso, usuario, PPID, línea de comandos y ruta del archivo durante una investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar procesos activos y sus identificadores para comprender qué aplicaciones y servicios están ejecutándose.

---

# PPID

**¿Qué es?**  
PPID (Parent Process ID) es el identificador del proceso que creó o inició un proceso determinado.

**¿Dónde lo encuentro?**  
En herramientas de análisis de procesos, EDR, Sysmon y otras fuentes de telemetría.

**¿Por qué me afecta?**  
Permite construir relaciones entre procesos y detectar cadenas de ejecución sospechosas.

**¿Cómo se soluciona?**  
Analizando si la relación entre proceso hijo y proceso padre es esperada y correlacionándola con el usuario, línea de comandos y contexto.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede abusar de procesos legítimos como padres o intentar ejecutar código mediante cadenas de procesos que parezcan normales.

---

# Service

**¿Qué es?**  
Service es un componente de software que puede ejecutarse en segundo plano y realizar funciones específicas sin requerir una interacción directa del usuario.

**¿Dónde lo encuentro?**  
En sistemas Windows, servidores, aplicaciones empresariales y herramientas de administración.

**¿Por qué me afecta?**  
Los servicios pueden ejecutarse con privilegios elevados y tener acceso continuo a recursos importantes del sistema.

**¿Cómo se soluciona?**  
Revisando los servicios instalados, limitando sus privilegios, deshabilitando los innecesarios y monitoreando cambios en su configuración.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar abusar de servicios existentes o establecer un servicio controlado por él para mantener ejecución o persistencia.

---

# Driver

**¿Qué es?**  
Driver es un componente de software que permite al sistema operativo comunicarse y controlar hardware u otros componentes de bajo nivel.

**¿Dónde lo encuentro?**  
En sistemas operativos, especialmente Windows, donde los drivers permiten interactuar con dispositivos y determinados componentes del sistema.

**¿Por qué me afecta?**  
Los drivers operan con privilegios elevados y una vulnerabilidad o driver malicioso puede comprometer componentes críticos del sistema.

**¿Cómo se soluciona?**  
Manteniendo los drivers actualizados, utilizando únicamente controladores confiables y aplicando mecanismos de seguridad que restrinjan drivers no autorizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar abusar de un driver vulnerable o cargar un driver malicioso para ejecutar acciones con privilegios elevados y evadir determinados controles de seguridad.
