# Active Directory

**¿Qué es?**  
Active Directory (AD) es el servicio de directorio de Microsoft que permite administrar de forma centralizada identidades, equipos, grupos, recursos y políticas dentro de un entorno Windows.

**¿Dónde lo encuentro?**  
Principalmente en redes empresariales Windows, donde uno o más Domain Controllers administran un dominio.

**¿Por qué me afecta?**  
Un compromiso de Active Directory puede proporcionar a un atacante acceso a múltiples sistemas, cuentas y recursos de la organización.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, protegiendo cuentas privilegiadas, monitoreando autenticaciones y cambios en AD y manteniendo actualizados los Domain Controllers.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar reconocimiento del directorio, comprometer credenciales y utilizar relaciones de confianza y permisos para desplazarse dentro del entorno.

---

# Domain Controller

**¿Qué es?**  
Domain Controller (DC) es un servidor que ejecuta los servicios de Active Directory y gestiona autenticación, autorización y otros servicios relacionados con el dominio.

**¿Dónde lo encuentro?**  
En infraestructuras Windows que utilizan Active Directory para administrar usuarios, equipos y recursos.

**¿Por qué me afecta?**  
Un Domain Controller comprometido puede poner en riesgo las identidades y recursos de gran parte del dominio.

**¿Cómo se soluciona?**  
Protegiéndolo con controles estrictos, restringiendo el acceso administrativo, monitoreando sus eventos y manteniendo sus servicios actualizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer cuentas privilegiadas o servicios que permitan alcanzar el Domain Controller y obtener un nivel elevado de control sobre el dominio.

---

# Domain

**¿Qué es?**  
Domain es una unidad lógica de administración dentro de Active Directory que agrupa usuarios, equipos, grupos y otros objetos bajo una estructura común de identidad y políticas.

**¿Dónde lo encuentro?**  
En entornos empresariales que utilizan Active Directory.

**¿Por qué me afecta?**  
El dominio establece relaciones de confianza y controles de acceso que determinan cómo los usuarios y equipos interactúan con los recursos de la organización.

**¿Cómo se soluciona?**  
Administrando correctamente las relaciones de confianza, permisos, políticas de seguridad y cuentas pertenecientes al dominio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explorar objetos y relaciones dentro del dominio para identificar cuentas, equipos, grupos y rutas potenciales de escalada de privilegios.

---

# Organizational Unit

**¿Qué es?**  
Organizational Unit (OU) es un contenedor dentro de Active Directory utilizado para organizar objetos como usuarios, grupos y equipos y aplicarles políticas de forma administrativa.

**¿Dónde lo encuentro?**  
En Active Directory, dentro de la estructura jerárquica de un dominio.

**¿Por qué me afecta?**  
Una configuración incorrecta de una OU o de sus políticas puede otorgar permisos excesivos o aplicar configuraciones inseguras a múltiples objetos.

**¿Cómo se soluciona?**  
Organizando las OUs de forma adecuada, aplicando políticas de seguridad correctamente y revisando permisos y delegaciones administrativas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar OUs con configuraciones o delegaciones débiles que le permitan obtener permisos adicionales.

---

# Group

**¿Qué es?**  
Group es un conjunto de cuentas u objetos de Active Directory utilizado para administrar permisos y acceso a recursos de forma colectiva.

**¿Dónde lo encuentro?**  
En Active Directory, sistemas Windows, aplicaciones empresariales y recursos que utilizan grupos para controlar acceso.

**¿Por qué me afecta?**  
La pertenencia incorrecta a un grupo puede otorgar a un usuario acceso a información o funciones que no debería tener.

**¿Cómo se soluciona?**  
Revisando periódicamente las membresías, aplicando mínimo privilegio y evitando privilegios administrativos innecesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar grupos privilegiados y cuentas que pertenezcan a ellos para identificar posibles rutas de escalada de privilegios.

---

# Domain User

**¿Qué es?**  
Domain User es una cuenta de usuario administrada por Active Directory que puede autenticarse en los sistemas y acceder a recursos según sus permisos.

**¿Dónde lo encuentro?**  
En Active Directory y en equipos o servicios que utilizan las identidades del dominio.

**¿Por qué me afecta?**  
Una cuenta de dominio comprometida puede proporcionar al atacante acceso a recursos adicionales dependiendo de sus permisos y relaciones.

**¿Cómo se soluciona?**  
Aplicando políticas de autenticación seguras, MFA cuando sea posible, mínimo privilegio, monitoreo de autenticaciones y gestión adecuada del ciclo de vida de las cuentas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener las credenciales de un Domain User y utilizar la cuenta para acceder a recursos del dominio.

---

# Service Account

**¿Qué es?**  
Service Account es una cuenta utilizada por un servicio, aplicación o proceso para autenticarse y realizar determinadas operaciones.

**¿Dónde lo encuentro?**  
En servidores, aplicaciones, servicios Windows, bases de datos, Active Directory y otros sistemas empresariales.

**¿Por qué me afecta?**  
Las cuentas de servicio suelen tener permisos necesarios para ejecutar aplicaciones y, si están configuradas con privilegios excesivos, pueden convertirse en objetivos importantes.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, utilizando mecanismos seguros de gestión de credenciales, rotando secretos y monitoreando su uso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una Service Account para aprovechar los permisos asignados al servicio y acceder a otros recursos.

---

# Computer Account

**¿Qué es?**  
Computer Account es el objeto de Active Directory que representa un equipo unido al dominio y permite establecer su identidad dentro del entorno.

**¿Dónde lo encuentro?**  
En Active Directory, asociado a estaciones de trabajo, servidores y otros equipos unidos al dominio.

**¿Por qué me afecta?**  
Una cuenta de equipo comprometida o mal configurada puede utilizarse para acceder a recursos del dominio o facilitar movimientos dentro de la red.

**¿Cómo se soluciona?**  
Controlando los equipos que pueden unirse al dominio, protegiendo sus credenciales, monitoreando cambios y eliminando cuentas de equipos que ya no estén en uso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer un equipo unido al dominio y aprovechar su identidad y relaciones con otros recursos para avanzar dentro del entorno.
