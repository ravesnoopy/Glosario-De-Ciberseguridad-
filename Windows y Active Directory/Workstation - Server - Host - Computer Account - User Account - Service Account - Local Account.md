# Workstation

**¿Qué es?**  
Workstation es un equipo utilizado principalmente por una persona para realizar actividades de trabajo, como ejecutar aplicaciones, acceder a recursos y procesar información.

**¿Dónde lo encuentro?**  
En redes empresariales, oficinas, entornos corporativos y organizaciones donde los empleados utilizan equipos para sus actividades diarias.

**¿Por qué me afecta?**  
Una Workstation comprometida puede proporcionar acceso a información, credenciales y recursos de red disponibles para el usuario.

**¿Cómo se soluciona?**  
Aplicando parches, EDR/antivirus, mínimo privilegio, controles de acceso, segmentación de red y monitoreo de actividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer una Workstation mediante phishing, malware, credenciales robadas o vulnerabilidades para obtener un punto de entrada a la organización.

---

# Server

**¿Qué es?**  
Server es un sistema que proporciona servicios, aplicaciones, almacenamiento, bases de datos u otros recursos a otros equipos o usuarios.

**¿Dónde lo encuentro?**  
En centros de datos, redes empresariales, entornos cloud y cualquier infraestructura que proporcione servicios centralizados.

**¿Por qué me afecta?**  
Un servidor comprometido puede afectar aplicaciones, datos o servicios utilizados por numerosos usuarios y sistemas.

**¿Cómo se soluciona?**  
Aplicando hardening, parches, segmentación, mínimo privilegio, monitoreo y controles de acceso adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar explotar vulnerabilidades, comprometer credenciales o abusar de servicios expuestos para obtener acceso al servidor.

---

# Host

**¿Qué es?**  
Host es cualquier dispositivo o sistema conectado a una red que puede enviar, recibir o procesar comunicaciones.

**¿Dónde lo encuentro?**  
En redes locales, Internet, entornos cloud y cualquier infraestructura conectada mediante una red.

**¿Por qué me afecta?**  
Cada host representa un posible punto de exposición y puede contener datos, servicios o credenciales importantes.

**¿Cómo se soluciona?**  
Manteniendo los hosts actualizados, reduciendo servicios innecesarios, aplicando controles de acceso y monitoreando su actividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar reconocimiento para identificar hosts activos, servicios disponibles y posibles puntos de entrada.

---

# Computer Account

**¿Qué es?**  
Computer Account es el objeto de Active Directory que representa la identidad de un equipo unido a un dominio.

**¿Dónde lo encuentro?**  
En Active Directory, asociado con Workstations, Servers y otros equipos unidos al dominio.

**¿Por qué me afecta?**  
La cuenta de equipo permite que el dispositivo se identifique y participe en las relaciones de confianza del dominio.

**¿Cómo se soluciona?**  
Controlando qué equipos pueden unirse al dominio, protegiendo sus credenciales, monitoreando cambios y eliminando cuentas de equipos que ya no estén en uso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer un equipo unido al dominio y aprovechar su identidad y relaciones para acceder a otros recursos.

---

# User Account

**¿Qué es?**  
User Account es una identidad utilizada por una persona o proceso para autenticarse en un sistema y acceder a recursos según los permisos asignados.

**¿Dónde lo encuentro?**  
En sistemas operativos, Active Directory, aplicaciones, servicios cloud y otros sistemas de gestión de identidades.

**¿Por qué me afecta?**  
Una cuenta comprometida puede proporcionar acceso a los recursos disponibles para esa identidad.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, autenticación fuerte, MFA cuando sea posible, gestión adecuada del ciclo de vida de las cuentas y monitoreo de accesos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede obtener o abusar de las credenciales de una cuenta para acceder a sistemas y recursos como si fuera el usuario legítimo.

---

# Service Account

**¿Qué es?**  
Service Account es una cuenta utilizada por un servicio, aplicación o proceso para autenticarse y realizar operaciones determinadas.

**¿Dónde lo encuentro?**  
En servidores, aplicaciones, servicios Windows, Active Directory, bases de datos y otros sistemas empresariales.

**¿Por qué me afecta?**  
Una Service Account puede tener permisos elevados o acceso a múltiples recursos necesarios para el funcionamiento de una aplicación.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, gestionando de forma segura sus credenciales, rotando secretos y monitoreando su actividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una Service Account y aprovechar los permisos asignados para acceder a otros sistemas o recursos.

---

# Local Account

**¿Qué es?**  
Local Account es una cuenta administrada directamente por un equipo y utilizada para autenticarse en ese sistema sin depender necesariamente de una identidad de Active Directory.

**¿Dónde lo encuentro?**  
En Workstations, Servers y otros sistemas que mantienen cuentas locales.

**¿Por qué me afecta?**  
Las cuentas locales, especialmente las administrativas, pueden proporcionar acceso directo al sistema y convertirse en objetivos para el robo de credenciales.

**¿Cómo se soluciona?**  
Eliminando cuentas innecesarias, aplicando mínimo privilegio, utilizando contraseñas únicas y robustas y gestionando adecuadamente las cuentas administrativas locales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una Local Account y utilizarla para obtener acceso al equipo o, si posee privilegios suficientes, realizar acciones administrativas.
