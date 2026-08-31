# SYSVOL

**¿Qué es?**  
SYSVOL es una carpeta compartida en los Domain Controllers que almacena archivos necesarios para distribuir determinadas políticas y configuraciones de Group Policy dentro de un dominio.

**¿Dónde lo encuentro?**  
En los Domain Controllers de un entorno Active Directory, normalmente accesible mediante una ruta de red asociada al dominio.

**¿Por qué me afecta?**  
Los archivos almacenados en SYSVOL pueden contener configuraciones y scripts utilizados por múltiples equipos del dominio, por lo que una modificación no autorizada puede tener un impacto amplio.

**¿Cómo se soluciona?**  
Protegiendo los permisos, monitoreando modificaciones y evitando almacenar información sensible, como contraseñas, dentro de archivos de políticas o scripts.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar información útil dentro de SYSVOL o intentar modificar archivos si obtiene permisos suficientes para afectar configuraciones distribuidas mediante Group Policy.

---

# NETLOGON

**¿Qué es?**  
NETLOGON es un servicio de Windows que participa en procesos de autenticación, comunicación entre equipos y Domain Controllers y determinadas operaciones relacionadas con el dominio.

**¿Dónde lo encuentro?**  
En equipos Windows unidos a un dominio y especialmente en Domain Controllers.

**¿Por qué me afecta?**  
Su funcionamiento es importante para las relaciones de confianza, autenticación y comunicación dentro de un entorno Active Directory.

**¿Cómo se soluciona?**  
Manteniendo Windows actualizado, protegiendo los Domain Controllers y monitoreando eventos relacionados con autenticación y actividad de dominio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar abusar de vulnerabilidades o configuraciones débiles relacionadas con los mecanismos de autenticación y comunicación del dominio.

---

# Kerberos

**¿Qué es?**  
Kerberos es un protocolo de autenticación utilizado por Active Directory para permitir que usuarios y servicios se autentiquen mediante tickets sin enviar directamente sus contraseñas a cada servicio.

**¿Dónde lo encuentro?**  
Principalmente en entornos Windows con Active Directory, donde los Domain Controllers actúan como Key Distribution Centers (KDC).

**¿Por qué me afecta?**  
Un problema con las credenciales, tickets o configuración de Kerberos puede afectar la autenticación y permitir accesos no autorizados.

**¿Cómo se soluciona?**  
Protegiendo las cuentas privilegiadas, utilizando contraseñas robustas, manteniendo sincronización de tiempo y monitoreando eventos de autenticación Kerberos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener o abusar de tickets y credenciales Kerberos para autenticarse como usuarios o servicios sin conocer necesariamente sus contraseñas.

---

# LDAP

**¿Qué es?**  
LDAP (Lightweight Directory Access Protocol) es un protocolo utilizado para consultar y administrar información almacenada en servicios de directorio, como Active Directory.

**¿Dónde lo encuentro?**  
En redes empresariales, Active Directory, aplicaciones y servicios que necesitan consultar información de usuarios, grupos y otros objetos.

**¿Por qué me afecta?**  
Consultas LDAP excesivas o acceso no autorizado pueden revelar información sobre usuarios, grupos, equipos y estructura del entorno.

**¿Cómo se soluciona?**  
Protegiendo las comunicaciones, restringiendo permisos, aplicando autenticación adecuada y monitoreando consultas anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede consultar LDAP para realizar reconocimiento y obtener información sobre usuarios, grupos, equipos y otros objetos del dominio.

---

# DNS

**¿Qué es?**  
DNS (Domain Name System) es el sistema que traduce nombres de dominio y nombres de host a direcciones IP y permite resolver diferentes tipos de registros utilizados por los servicios de red.

**¿Dónde lo encuentro?**  
En redes locales, Internet, servidores DNS, Domain Controllers y dispositivos que necesitan resolver nombres.

**¿Por qué me afecta?**  
DNS es fundamental para la conectividad y también puede proporcionar información sobre infraestructura o ser utilizado para transportar comunicaciones no autorizadas.

**¿Cómo se soluciona?**  
Protegiendo los servidores DNS, controlando las consultas, monitoreando dominios sospechosos y aplicando políticas de resolución adecuadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar DNS para realizar reconocimiento, resolver infraestructura maliciosa o establecer canales de comunicación encubiertos.

---

# SMB Share

**¿Qué es?**  
SMB Share es un recurso compartido mediante el protocolo SMB que permite acceder a archivos, carpetas u otros recursos a través de una red.

**¿Dónde lo encuentro?**  
En servidores y equipos Windows, redes empresariales y entornos Active Directory.

**¿Por qué me afecta?**  
Los recursos compartidos con permisos excesivos pueden exponer información sensible o permitir modificaciones no autorizadas.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, revisando permisos de los recursos compartidos, restringiendo accesos innecesarios y utilizando versiones seguras de SMB.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar recursos compartidos, buscar información sensible y aprovechar permisos excesivos para acceder o modificar archivos dentro de la red.
