
## AS-REQ

**¿Qué es?**  
AS-REQ (Authentication Service Request) es un mensaje del protocolo Kerberos que un cliente envía al Authentication Server (AS) para solicitar un Ticket Granting Ticket (TGT).

**¿Dónde lo encuentro?**  
En entornos Windows con Active Directory y Kerberos, donde los clientes solicitan autenticación al controlador de dominio.

**¿Por qué me afecta?**  
Los AS-REQ forman parte del proceso de autenticación de Kerberos y pueden proporcionar evidencia útil para detectar comportamientos anómalos, como intentos masivos de autenticación.

**¿Cómo se soluciona?**  
Monitoreando eventos de autenticación de Kerberos, aplicando contraseñas robustas, MFA cuando sea compatible y protegiendo las cuentas privilegiadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar solicitudes AS-REQ para intentar obtener material relacionado con la autenticación y realizar ataques contra cuentas que utilicen métodos de Kerberos vulnerables.

## AS-REP

**¿Qué es?**  
AS-REP (Authentication Service Reply) es la respuesta del Authentication Server a un AS-REQ. Normalmente contiene información que permite al cliente obtener un TGT cuando la autenticación es válida.

**¿Dónde lo encuentro?**  
En las comunicaciones Kerberos entre clientes y controladores de dominio dentro de entornos Active Directory.

**¿Por qué me afecta?**  
Las respuestas AS-REP pueden ser relevantes para la seguridad cuando existen cuentas configuradas sin requerir preautenticación de Kerberos.

**¿Cómo se soluciona?**  
Habilitando la preautenticación Kerberos en las cuentas que la requieren, utilizando contraseñas robustas y monitoreando solicitudes AS-REP inusuales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede solicitar respuestas AS-REP de cuentas que no requieren preautenticación y utilizar la información obtenida para intentar recuperar la contraseña mediante técnicas de cracking offline.

## TGS-REQ

**¿Qué es?**  
TGS-REQ (Ticket Granting Service Request) es un mensaje Kerberos utilizado por un cliente para solicitar un ticket de servicio al Ticket Granting Service (TGS).

**¿Dónde lo encuentro?**  
En entornos Active Directory cuando un usuario o servicio autenticado necesita acceder a un recurso protegido por Kerberos.

**¿Por qué me afecta?**  
Las solicitudes TGS-REQ son parte normal de Kerberos, pero patrones anómalos pueden revelar intentos de enumerar servicios o cuentas de servicio.

**¿Cómo se soluciona?**  
Protegiendo las cuentas de servicio, utilizando contraseñas robustas o administradas, aplicando mínimo privilegio y monitoreando solicitudes Kerberos inusuales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede solicitar múltiples tickets de servicio asociados con cuentas de servicio y utilizar la información obtenida para intentar recuperar sus contraseñas mediante ataques offline.

## TGS-REP

**¿Qué es?**  
TGS-REP (Ticket Granting Service Reply) es la respuesta del TGS a una solicitud TGS-REQ y contiene el ticket que permite al cliente acceder al servicio solicitado.

**¿Dónde lo encuentro?**  
En las comunicaciones Kerberos de entornos Active Directory cuando un cliente solicita acceso a servicios como SMB, LDAP o MSSQL.

**¿Por qué me afecta?**  
Los TGS-REP son importantes para la seguridad de Kerberos porque pueden contener información que un atacante podría intentar utilizar para atacar las credenciales de cuentas de servicio.

**¿Cómo se soluciona?**  
Utilizando cuentas de servicio con contraseñas robustas o administradas, evitando privilegios innecesarios y monitoreando patrones anómalos de solicitudes de tickets.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede solicitar tickets para determinadas cuentas de servicio y utilizar las respuestas obtenidas en ataques de **Kerberoasting** para intentar recuperar sus contraseñas offline.
