
## DCSync

**¿Qué es?**  
DCSync es una técnica que abusa de los permisos de replicación de Active Directory para solicitar datos de credenciales desde un controlador de dominio como si fuera otro controlador.

**¿Dónde lo encuentro?**  
En entornos Windows con Active Directory, especialmente cuando una cuenta comprometida posee permisos de replicación excesivos o equivalentes a los utilizados por los controladores de dominio.

**¿Por qué me afecta?**  
Puede permitir obtener material de autenticación de numerosas cuentas del dominio, incluyendo cuentas altamente privilegiadas, sin necesidad de acceder directamente al controlador de dominio.

**¿Cómo se soluciona?**  
Restringiendo los permisos de replicación, aplicando mínimo privilegio, protegiendo cuentas privilegiadas y monitoreando solicitudes de replicación anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar una cuenta con permisos de replicación comprometida para solicitar información de credenciales y obtener material que le permita comprometer otras cuentas del dominio.

## Golden Ticket

**¿Qué es?**  
Golden Ticket es una técnica que permite crear un TGT de Kerberos falsificado utilizando el material secreto de la cuenta `krbtgt` de un dominio comprometido.

**¿Dónde lo encuentro?**  
En entornos Active Directory donde la cuenta `krbtgt` o sus secretos de autenticación han sido comprometidos.

**¿Por qué me afecta?**  
Puede proporcionar persistencia y acceso amplio dentro del dominio, incluso después de que se hayan restablecido otras credenciales.

**¿Cómo se soluciona?**  
Protegiendo la cuenta `krbtgt`, reduciendo privilegios administrativos, detectando anomalías en tickets Kerberos y restableciendo adecuadamente la contraseña de `krbtgt` durante una respuesta a compromiso.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de obtener el secreto de `krbtgt`, puede crear tickets Kerberos falsificados para intentar autenticarse como usuarios y acceder a recursos del dominio.

## Silver Ticket

**¿Qué es?**  
Silver Ticket es una técnica que consiste en crear un ticket de servicio Kerberos falsificado utilizando el secreto de una cuenta asociada a un servicio específico.

**¿Dónde lo encuentro?**  
En entornos Active Directory donde un atacante ha obtenido las credenciales o secretos de una cuenta de servicio utilizada por Kerberos.

**¿Por qué me afecta?**  
Puede permitir acceso no autorizado a un servicio específico y proporcionar persistencia sin necesidad de interactuar directamente con el controlador de dominio para cada acceso.

**¿Cómo se soluciona?**  
Protegiendo las cuentas de servicio, utilizando contraseñas robustas o administradas, aplicando mínimo privilegio y monitoreando autenticaciones Kerberos anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar el secreto de una cuenta de servicio comprometida para generar un ticket falsificado y acceder al servicio asociado con permisos de esa cuenta.

## Skeleton Key

**¿Qué es?**  
Skeleton Key es una técnica que modifica un controlador de dominio en memoria para aceptar una contraseña adicional que permite autenticarse como diferentes usuarios.

**¿Dónde lo encuentro?**  
En controladores de dominio Windows comprometidos donde un atacante ha conseguido privilegios suficientes para modificar procesos relacionados con la autenticación.

**¿Por qué me afecta?**  
Puede proporcionar acceso persistente a múltiples cuentas sin modificar sus contraseñas almacenadas, dificultando la identificación del compromiso mediante revisiones convencionales.

**¿Cómo se soluciona?**  
Protegiendo los controladores de dominio, limitando privilegios administrativos, monitoreando procesos críticos y realizando una recuperación confiable del controlador comprometido.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar el proceso de autenticación en memoria para aceptar una contraseña controlada por él y utilizarla para acceder a múltiples cuentas del dominio.
