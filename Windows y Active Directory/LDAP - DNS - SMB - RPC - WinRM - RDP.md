# LDAP

**¿Qué es?**  
LDAP (Lightweight Directory Access Protocol) es un protocolo utilizado para consultar y administrar información almacenada en servicios de directorio, como Active Directory.

**¿Dónde lo encuentro?**  
En redes empresariales, Active Directory, aplicaciones y servicios que necesitan consultar usuarios, grupos, equipos y otros objetos del directorio.

**¿Por qué me afecta?**  
LDAP puede proporcionar información importante sobre la estructura de un entorno y sus identidades. Una configuración insegura puede permitir consultas o accesos que deberían estar restringidos.

**¿Cómo se soluciona?**  
Aplicando controles de acceso adecuados, protegiendo las comunicaciones mediante LDAP seguro cuando corresponda y monitoreando consultas anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar consultas LDAP para obtener información sobre usuarios, grupos, equipos y otros objetos que le ayuden durante el reconocimiento.

---

# DNS

**¿Qué es?**  
DNS (Domain Name System) es el sistema que permite resolver nombres de dominio y nombres de host en direcciones IP y otros registros de red.

**¿Dónde lo encuentro?**  
En redes locales, Internet, servidores DNS, Domain Controllers y dispositivos que necesitan resolver nombres.

**¿Por qué me afecta?**  
DNS es fundamental para la conectividad y puede revelar información sobre infraestructura. También puede ser utilizado como canal de comunicación por software malicioso.

**¿Cómo se soluciona?**  
Protegiendo los servidores DNS, controlando las consultas, aplicando políticas de resolución y monitoreando dominios y patrones de consultas sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar DNS para realizar reconocimiento, resolver infraestructura controlada por el atacante o establecer comunicaciones encubiertas.

---

# SMB

**¿Qué es?**  
SMB (Server Message Block) es un protocolo utilizado principalmente para compartir archivos, carpetas, impresoras y otros recursos a través de una red.

**¿Dónde lo encuentro?**  
En sistemas Windows, servidores de archivos, estaciones de trabajo y entornos Active Directory.

**¿Por qué me afecta?**  
Una configuración insegura de SMB puede exponer recursos compartidos o facilitar el acceso no autorizado y el movimiento lateral.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, restringiendo el acceso a recursos compartidos, utilizando versiones seguras de SMB y monitoreando conexiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar recursos compartidos, buscar información sensible o utilizar credenciales comprometidas para acceder a otros sistemas mediante SMB.

---

# RPC

**¿Qué es?**  
RPC (Remote Procedure Call) es un mecanismo que permite a un programa solicitar la ejecución de operaciones en otro proceso o sistema.

**¿Dónde lo encuentro?**  
En sistemas Windows, servicios de red, aplicaciones distribuidas y componentes de Active Directory.

**¿Por qué me afecta?**  
Numerosos servicios de Windows dependen de RPC, por lo que una exposición o configuración insegura puede aumentar la superficie de ataque.

**¿Cómo se soluciona?**  
Restringiendo el acceso mediante segmentación y firewall, manteniendo los sistemas actualizados y monitoreando comunicaciones RPC relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar servicios RPC accesibles para realizar reconocimiento, interactuar con sistemas remotos o aprovechar vulnerabilidades conocidas.

---

# WinRM

**¿Qué es?**  
WinRM (Windows Remote Management) es el servicio de Windows que permite realizar administración remota de equipos mediante el estándar WS-Management.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows utilizados para administración remota, especialmente en entornos empresariales.

**¿Por qué me afecta?**  
Una configuración insegura o una exposición innecesaria de WinRM puede proporcionar una vía de administración remota que podría ser abusada.

**¿Cómo se soluciona?**  
Restringiendo qué usuarios y equipos pueden utilizar WinRM, protegiendo las credenciales y monitoreando las conexiones de administración remota.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para autenticarse remotamente y ejecutar acciones administrativas en otros equipos.

---

# RDP

**¿Qué es?**  
RDP (Remote Desktop Protocol) es un protocolo de Microsoft que permite acceder remotamente a un sistema Windows mediante una sesión gráfica.

**¿Dónde lo encuentro?**  
En servidores y equipos Windows donde se encuentra habilitado el acceso mediante Remote Desktop.

**¿Por qué me afecta?**  
Una cuenta comprometida o una configuración insegura de RDP puede proporcionar acceso interactivo a un sistema y facilitar movimientos laterales.

**¿Cómo se soluciona?**  
Restringiendo el acceso mediante firewall o VPN, utilizando MFA cuando sea posible, aplicando mínimo privilegio y monitoreando los inicios de sesión.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para establecer una sesión RDP y operar sobre el sistema con los permisos de la cuenta comprometida.
