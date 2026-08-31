# Active Directory

**¿Qué es?**  
Active Directory (AD) es el servicio de directorio de Microsoft que permite administrar de forma centralizada usuarios, equipos, grupos, recursos y políticas de seguridad dentro de un entorno Windows.

**¿Dónde lo encuentro?**  
En redes empresariales Windows donde se utiliza un dominio para centralizar la administración de identidades y recursos.

**¿Por qué me afecta?**  
Active Directory concentra información y controles de acceso de numerosos recursos. Un compromiso importante de AD puede afectar gran parte de la infraestructura.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, protegiendo cuentas privilegiadas, monitoreando autenticaciones y cambios administrativos y manteniendo actualizados los Domain Controllers.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar reconocimiento del dominio, comprometer credenciales y aprovechar permisos o relaciones de confianza para avanzar hacia recursos de mayor privilegio.

---

# Domain

**¿Qué es?**  
Domain es una unidad lógica de administración dentro de Active Directory que agrupa usuarios, equipos, grupos y otros objetos bajo una estructura común de identidad, autenticación y políticas.

**¿Dónde lo encuentro?**  
En entornos empresariales que utilizan Active Directory.

**¿Por qué me afecta?**  
El dominio establece cómo se administran las identidades y cómo los usuarios y equipos acceden a los recursos de la organización.

**¿Cómo se soluciona?**  
Administrando correctamente las cuentas, grupos, permisos, relaciones de confianza y políticas de seguridad del dominio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar usuarios, grupos, equipos y relaciones dentro del dominio para identificar posibles rutas de acceso o escalada de privilegios.

---

# Domain Controller

**¿Qué es?**  
Domain Controller (DC) es un servidor que ejecuta Active Directory Domain Services (AD DS) y proporciona servicios fundamentales de autenticación, autorización y administración del dominio.

**¿Dónde lo encuentro?**  
En entornos Active Directory. Normalmente existen uno o más Domain Controllers para proporcionar servicios de dominio y redundancia.

**¿Por qué me afecta?**  
El Domain Controller es un componente crítico porque administra información relacionada con las identidades y autenticación del dominio.

**¿Cómo se soluciona?**  
Restringiendo el acceso administrativo, protegiendo las cuentas privilegiadas, aplicando actualizaciones de seguridad y monitoreando eventos y cambios realizados en los Domain Controllers.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer credenciales privilegiadas y alcanzar el Domain Controller para obtener un nivel de control elevado sobre el dominio.

---

# Domain Admin

**¿Qué es?**  
Domain Admin es una cuenta o miembro del grupo **Domain Admins** que posee privilegios administrativos elevados sobre el dominio de Active Directory.

**¿Dónde lo encuentro?**  
En Active Directory, dentro del grupo de seguridad **Domain Admins**.

**¿Por qué me afecta?**  
Una cuenta Domain Admin tiene un nivel de privilegio muy alto y su compromiso puede permitir al atacante controlar numerosos sistemas y recursos del dominio.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, restringiendo la membresía de Domain Admins, utilizando cuentas administrativas separadas, protegiendo las credenciales y monitoreando actividades privilegiadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una cuenta Domain Admin mediante robo de credenciales, abuso de sesiones o escalada de privilegios para obtener control administrativo sobre el dominio.
