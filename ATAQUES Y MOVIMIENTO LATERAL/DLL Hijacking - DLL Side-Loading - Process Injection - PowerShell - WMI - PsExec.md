
## DLL Hijacking

**¿Qué es?**  
DLL Hijacking es una técnica en la que un atacante consigue que una aplicación cargue una DLL maliciosa en lugar de la DLL legítima que esperaba encontrar.

**¿Dónde lo encuentro?**  
En sistemas Windows y aplicaciones que buscan DLLs en ubicaciones donde un atacante puede colocar o controlar archivos.

**¿Por qué me afecta?**  
Puede permitir la ejecución de código malicioso con los permisos del proceso legítimo y facilitar persistencia o escalación de privilegios.

**¿Cómo se soluciona?**  
Manteniendo el software actualizado, restringiendo permisos de escritura en directorios sensibles y configurando las aplicaciones para cargar DLLs desde ubicaciones confiables.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede colocar una DLL maliciosa en una ubicación que tenga prioridad durante la búsqueda de DLLs para lograr que una aplicación legítima la ejecute.

## DLL Side-Loading

**¿Qué es?**  
DLL Side-Loading es una técnica que abusa de una aplicación legítima para cargar una DLL maliciosa que comparte el nombre esperado por el programa.

**¿Dónde lo encuentro?**  
En sistemas Windows donde aplicaciones legítimas utilizan DLLs y el orden de búsqueda permite que una biblioteca controlada por el atacante sea cargada.

**¿Por qué me afecta?**  
Permite ejecutar código malicioso mediante un ejecutable legítimo, lo que puede dificultar su detección y facilitar técnicas de evasión.

**¿Cómo se soluciona?**  
Manteniendo las aplicaciones actualizadas, restringiendo permisos de escritura y configurando mecanismos seguros para la carga de DLLs.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede colocar una DLL maliciosa junto a un ejecutable legítimo para conseguir que este la cargue y ejecute el código contenido en ella.

## Process Injection

**¿Qué es?**  
Process Injection es una técnica mediante la cual un proceso malicioso introduce código en otro proceso para ejecutar acciones dentro de su espacio de memoria.

**¿Dónde lo encuentro?**  
En sistemas Windows y otras plataformas donde un proceso puede interactuar con la memoria o ejecución de otro proceso.

**¿Por qué me afecta?**  
Puede permitir que código malicioso se ejecute dentro de un proceso legítimo, dificultando la detección y facilitando evasión de controles de seguridad.

**¿Cómo se soluciona?**  
Utilizando controles de seguridad del endpoint, restringiendo privilegios, monitoreando comportamientos anómalos entre procesos y manteniendo sistemas y aplicaciones actualizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede inyectar código en un proceso legítimo para ejecutar acciones maliciosas utilizando su contexto y tratar de ocultar la actividad.

## PowerShell

**¿Qué es?**  
PowerShell es una herramienta y entorno de automatización y administración de sistemas de Windows basado en comandos y scripts.

**¿Dónde lo encuentro?**  
En sistemas Windows, estaciones de trabajo, servidores y entornos empresariales donde se utiliza para administración y automatización.

**¿Por qué me afecta?**  
Sus capacidades legítimas de administración y ejecución de scripts pueden ser abusadas para ejecutar código, recopilar información o automatizar actividades maliciosas.

**¿Cómo se soluciona?**  
Aplicando controles de ejecución, políticas de seguridad, registro de actividad, restricciones de privilegios y monitoreo de comandos y procesos sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar PowerShell para ejecutar scripts, recopilar información, descargar componentes maliciosos o realizar acciones posteriores al compromiso.

## WMI

**¿Qué es?**  
WMI (Windows Management Instrumentation) es una infraestructura de Windows que permite consultar y administrar componentes y recursos del sistema mediante programación.

**¿Dónde lo encuentro?**  
En sistemas Windows, estaciones de trabajo, servidores y herramientas administrativas que necesitan consultar o gestionar recursos del sistema.

**¿Por qué me afecta?**  
Sus capacidades administrativas pueden ser abusadas para ejecutar acciones, recopilar información y realizar movimientos dentro de una red.

**¿Cómo se soluciona?**  
Limitando privilegios, controlando quién puede acceder a WMI, segmentando la red y monitoreando actividades y procesos asociados con su uso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar WMI para recopilar información del sistema, ejecutar acciones remotamente o desplazarse hacia otros equipos comprometidos.

## PsExec

**¿Qué es?**  
PsExec es una herramienta de administración de Windows que permite ejecutar procesos en sistemas remotos mediante mecanismos propios del sistema operativo.

**¿Dónde lo encuentro?**  
En entornos Windows donde administradores utilizan herramientas de administración remota para gestionar estaciones de trabajo y servidores.

**¿Por qué me afecta?**  
Aunque tiene usos legítimos, su capacidad de ejecución remota puede ser abusada para realizar movimiento lateral dentro de una red.

**¿Cómo se soluciona?**  
Restringiendo la administración remota, aplicando mínimo privilegio, controlando cuentas administrativas y monitoreando ejecuciones remotas y creación de servicios.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de obtener credenciales con privilegios suficientes, puede utilizar PsExec para ejecutar procesos en otros equipos y desplazarse lateralmente por la red.
