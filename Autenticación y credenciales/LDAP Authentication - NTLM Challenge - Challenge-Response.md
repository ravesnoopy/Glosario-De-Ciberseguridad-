
## LDAP Authentication

**¿Qué es?**  
LDAP Authentication es el proceso mediante el cual un usuario, aplicación o servicio verifica sus credenciales contra un directorio LDAP para obtener acceso a recursos.

**¿Dónde lo encuentro?**  
En Active Directory, servidores LDAP, aplicaciones empresariales, VPN, sistemas de correo y servicios que utilizan directorios centralizados para gestionar identidades.

**¿Por qué me afecta?**  
Una configuración insegura puede permitir exposición de credenciales, accesos no autorizados o comunicaciones sin protección entre el cliente y el servidor LDAP.

**¿Cómo se soluciona?**  
Utilizando LDAP sobre TLS, métodos de autenticación seguros, mínimo privilegio y controles adecuados para proteger las cuentas y las comunicaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar capturar credenciales, abusar de configuraciones LDAP inseguras o utilizar cuentas comprometidas para consultar información del directorio.

## NTLM Challenge

**¿Qué es?**  
NTLM Challenge es una etapa del mecanismo de autenticación NTLM en la que el servidor envía un valor aleatorio denominado challenge al cliente para participar en la verificación de sus credenciales.

**¿Dónde lo encuentro?**  
En sistemas Windows y servicios que utilizan NTLM para autenticación, especialmente en entornos donde todavía existen aplicaciones o sistemas heredados.

**¿Por qué me afecta?**  
Las autenticaciones NTLM pueden ser objetivo de ataques de relay, captura de material de autenticación y cracking offline dependiendo del contexto y la configuración.

**¿Cómo se soluciona?**  
Reduciendo el uso de NTLM cuando sea posible, priorizando Kerberos, habilitando protecciones contra relay y monitoreando autenticaciones NTLM anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar provocar una autenticación NTLM y capturar el intercambio challenge-response para utilizarlo en ataques de relay o intentar recuperar la contraseña mediante cracking offline.

## Challenge-Response

**¿Qué es?**  
Challenge-Response es un mecanismo de autenticación en el que un servidor envía un valor aleatorio y el cliente genera una respuesta basada en ese valor y en un secreto compartido, sin enviar directamente la contraseña.

**¿Dónde lo encuentro?**  
En protocolos y sistemas de autenticación como NTLM y otros mecanismos diseñados para verificar identidades sin transmitir la contraseña en texto claro.

**¿Por qué me afecta?**  
Aunque evita enviar directamente la contraseña, el intercambio puede ser atacado mediante relay, cracking offline u otras técnicas dependiendo del protocolo utilizado.

**¿Cómo se soluciona?**  
Utilizando protocolos modernos y resistentes a relay, protegiendo las comunicaciones, aplicando MFA cuando sea posible y reduciendo el uso de mecanismos heredados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede capturar un intercambio Challenge-Response y tratar de reutilizarlo contra otro servicio o analizarlo offline para intentar obtener las credenciales.
