# Scheduled Task

**¿Qué es?**  
Scheduled Task es una tarea configurada en Windows para ejecutar automáticamente un programa, script o comando en un momento determinado o cuando ocurre un evento específico.

**¿Dónde lo encuentro?**  
En Windows mediante Task Scheduler (`taskschd.msc`), herramientas administrativas y registros relacionados con tareas programadas.

**¿Por qué me afecta?**  
Las tareas programadas pueden ejecutar procesos legítimos automáticamente, pero una configuración no autorizada puede utilizarse para mantener persistencia o ejecutar código.

**¿Cómo se soluciona?**  
Revisando periódicamente las tareas existentes, eliminando las no autorizadas y monitoreando su creación y modificación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede crear o modificar una tarea para ejecutar código automáticamente y mantener persistencia en el sistema.

---

# Startup Folder

**¿Qué es?**  
Startup Folder es una carpeta de Windows cuyo contenido puede ejecutarse automáticamente cuando un usuario inicia sesión.

**¿Dónde lo encuentro?**  
En perfiles de usuario de Windows y en ubicaciones utilizadas por el sistema para iniciar aplicaciones automáticamente.

**¿Por qué me afecta?**  
Un archivo colocado de forma no autorizada puede ejecutarse cada vez que un usuario inicia sesión.

**¿Cómo se soluciona?**  
Monitoreando los archivos de las carpetas de inicio, restringiendo permisos y eliminando elementos desconocidos o innecesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede colocar un programa o script en una ubicación de inicio para conseguir ejecución automática después del inicio de sesión.

---

# Run Key

**¿Qué es?**  
Run Key es una clave del Windows Registry utilizada para especificar programas que deben ejecutarse automáticamente cuando un usuario inicia sesión.

**¿Dónde lo encuentro?**  
En el Windows Registry, dentro de las claves relacionadas con el inicio automático de aplicaciones.

**¿Por qué me afecta?**  
Una modificación no autorizada puede provocar que un programa se ejecute automáticamente durante el inicio de sesión.

**¿Cómo se soluciona?**  
Monitoreando las claves de inicio automático, restringiendo modificaciones y revisando cualquier entrada desconocida.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede agregar una entrada al Registry para ejecutar un programa controlado por él cada vez que una cuenta inicia sesión.

---

# WMI

**¿Qué es?**  
WMI (Windows Management Instrumentation) es una tecnología de Windows que permite administrar y consultar información sobre sistemas, procesos, servicios y otros componentes.

**¿Dónde lo encuentro?**  
En sistemas Windows, herramientas administrativas, scripts y aplicaciones de administración.

**¿Por qué me afecta?**  
WMI proporciona capacidades administrativas legítimas que pueden ser abusadas para ejecutar acciones, consultar sistemas o realizar administración remota.

**¿Cómo se soluciona?**  
Restringiendo permisos, monitoreando actividades WMI y registrando operaciones administrativas relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede abusar de WMI para ejecutar acciones, recopilar información o interactuar remotamente con sistemas comprometidos.

---

# WinRM

**¿Qué es?**  
WinRM (Windows Remote Management) es el servicio de Windows que permite administrar sistemas de forma remota mediante protocolos basados en WS-Management.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows utilizados para administración remota.

**¿Por qué me afecta?**  
Una configuración o exposición incorrecta de WinRM puede proporcionar una vía de acceso remoto no autorizada.

**¿Cómo se soluciona?**  
Restringiendo quién puede utilizar WinRM, limitando los equipos autorizados, protegiendo las credenciales y monitoreando conexiones remotas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para acceder remotamente a sistemas mediante WinRM.

---

# SMB

**¿Qué es?**  
SMB (Server Message Block) es un protocolo utilizado principalmente para compartir archivos, impresoras y otros recursos a través de una red.

**¿Dónde lo encuentro?**  
En redes Windows, servidores de archivos, estaciones de trabajo y entornos Active Directory.

**¿Por qué me afecta?**  
Una configuración insegura de SMB puede permitir acceso no autorizado a recursos compartidos o facilitar movimientos dentro de una red.

**¿Cómo se soluciona?**  
Restringiendo el acceso, utilizando versiones seguras del protocolo, aplicando mínimo privilegio y monitoreando conexiones SMB.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar SMB para descubrir recursos compartidos, acceder a archivos o desplazarse lateralmente mediante credenciales comprometidas.

---

# RDP

**¿Qué es?**  
RDP (Remote Desktop Protocol) es un protocolo de Microsoft que permite conectarse remotamente a un equipo Windows mediante una interfaz gráfica.

**¿Dónde lo encuentro?**  
En servidores y equipos Windows que tienen habilitado el acceso remoto.

**¿Por qué me afecta?**  
Una cuenta comprometida o una configuración insegura de RDP puede proporcionar acceso remoto interactivo a un sistema.

**¿Cómo se soluciona?**  
Restringiendo el acceso mediante firewall y VPN, utilizando MFA cuando sea posible, aplicando mínimo privilegio y monitoreando los inicios de sesión.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para iniciar una sesión remota y operar sobre un sistema como un usuario legítimo.

---

# RPC

**¿Qué es?**  
RPC (Remote Procedure Call) es un mecanismo que permite que un programa solicite la ejecución de operaciones o servicios en otro proceso o sistema.

**¿Dónde lo encuentro?**  
En sistemas Windows, aplicaciones distribuidas, servicios de red y componentes de Active Directory.

**¿Por qué me afecta?**  
Muchos servicios de Windows dependen de RPC, por lo que una exposición o configuración insegura puede aumentar la superficie de ataque.

**¿Cómo se soluciona?**  
Restringiendo el acceso a servicios RPC, utilizando firewalls y segmentación de red y manteniendo los sistemas actualizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar servicios RPC accesibles para realizar reconocimiento, interactuar con sistemas remotos o aprovechar vulnerabilidades conocidas.

---

# Windows Firewall

**¿Qué es?**  
Windows Firewall es el firewall integrado de Windows que controla conexiones de red entrantes y salientes según reglas configuradas.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows mediante Windows Defender Firewall y sus herramientas de administración.

**¿Por qué me afecta?**  
Una configuración adecuada puede impedir conexiones no autorizadas y reducir la exposición de servicios.

**¿Cómo se soluciona?**  
Aplicando reglas restrictivas, permitiendo únicamente el tráfico necesario y revisando periódicamente las reglas existentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar reglas demasiado permisivas o, si obtiene privilegios administrativos, modificar el firewall para permitir comunicaciones no autorizadas.

---

# Defender

**¿Qué es?**  
Defender es el conjunto de tecnologías de seguridad de Microsoft orientadas a proteger sistemas Windows y otros recursos frente a diferentes amenazas.

**¿Dónde lo encuentro?**  
En ecosistemas Microsoft, incluyendo endpoints, servidores y servicios de seguridad administrados.

**¿Por qué me afecta?**  
Proporciona capacidades de prevención, detección y respuesta que ayudan a identificar y bloquear actividades maliciosas.

**¿Cómo se soluciona?**  
Manteniendo sus componentes actualizados, configurando correctamente las políticas y verificando que las protecciones estén activas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evadir, deshabilitar o degradar los mecanismos de protección de Defender después de obtener los privilegios necesarios.

---

# Defender Antivirus

**¿Qué es?**  
Defender Antivirus es el componente antimalware de Microsoft Defender encargado de detectar, bloquear y ayudar a eliminar software malicioso.

**¿Dónde lo encuentro?**  
En sistemas Windows compatibles y entornos administrados mediante las herramientas de seguridad de Microsoft.

**¿Por qué me afecta?**  
Ayuda a prevenir la ejecución de malware y detectar archivos o comportamientos asociados con amenazas.

**¿Cómo se soluciona?**  
Manteniendo actualizadas las firmas y componentes de protección, habilitando las capacidades de seguridad disponibles y configurando políticas adecuadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evitar la detección mediante técnicas de evasión o modificar configuraciones de seguridad si consigue privilegios suficientes.

---

# Defender Firewall

**¿Qué es?**  
Defender Firewall es el componente de Microsoft que controla el tráfico de red permitido o bloqueado mediante reglas de firewall en Windows.

**¿Dónde lo encuentro?**  
En sistemas Windows y herramientas de administración de Microsoft.

**¿Por qué me afecta?**  
Puede limitar conexiones no autorizadas y reducir la superficie de ataque de un equipo o servidor.

**¿Cómo se soluciona?**  
Configurando reglas basadas en mínimo privilegio, restringiendo servicios innecesarios y monitoreando cambios en las reglas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar reglas permisivas o intentar modificar la configuración del firewall para permitir conexiones que faciliten sus actividades.
