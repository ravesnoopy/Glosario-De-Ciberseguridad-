
## Password Hash

**¿Qué es?**  
Un Password Hash es el resultado de aplicar una función hash a una contraseña para almacenarla o utilizarla en procesos de autenticación sin guardar necesariamente la contraseña en texto claro.

**¿Dónde lo encuentro?**  
En bases de datos de aplicaciones, sistemas operativos, directorios de usuarios y mecanismos de autenticación que almacenan representaciones derivadas de las contraseñas.

**¿Por qué me afecta?**  
Si los hashes son obtenidos por un atacante, pueden intentar recuperar las contraseñas mediante ataques de diccionario, fuerza bruta o cracking offline.

**¿Cómo se soluciona?**  
Utilizando algoritmos diseñados para almacenar contraseñas, como Argon2, bcrypt o scrypt, junto con salts únicos y configuraciones de costo adecuadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar hashes de contraseñas y analizarlos offline para recuperar las contraseñas originales o reutilizar determinados tipos de hashes en ataques de autenticación.

## NTLM

**¿Qué es?**  
NTLM (NT LAN Manager) es una familia de protocolos de autenticación de Microsoft basada en un mecanismo Challenge-Response y utilizada principalmente en entornos Windows.

**¿Dónde lo encuentro?**  
En sistemas Windows, dominios Active Directory y aplicaciones o servicios que todavía requieren compatibilidad con autenticación NTLM.

**¿Por qué me afecta?**  
NTLM es una tecnología heredada con riesgos conocidos y puede ser objetivo de ataques como NTLM relay, Pass-the-Hash y cracking de material de autenticación.

**¿Cómo se soluciona?**  
Reduciendo o deshabilitando NTLM cuando sea posible, priorizando Kerberos, aplicando protecciones contra relay y monitoreando autenticaciones NTLM.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede capturar o robar material de autenticación NTLM y utilizarlo para intentar autenticarse, realizar relay o recuperar credenciales.

## NTLMv1

**¿Qué es?**  
NTLMv1 es una versión antigua del protocolo NTLM que utiliza mecanismos criptográficos débiles y actualmente se considera insegura.

**¿Dónde lo encuentro?**  
Principalmente en sistemas Windows y aplicaciones heredadas que mantienen compatibilidad con mecanismos antiguos de autenticación.

**¿Por qué me afecta?**  
Sus debilidades permiten que el material de autenticación sea más susceptible a captura, cracking y otros ataques.

**¿Cómo se soluciona?**  
Deshabilitando NTLMv1, migrando a protocolos modernos como Kerberos y eliminando dependencias de sistemas heredados cuando sea posible.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede capturar intercambios NTLMv1 y aprovechar sus debilidades para intentar recuperar credenciales o utilizarlos en ataques de autenticación.

## NTLMv2

**¿Qué es?**  
NTLMv2 es una versión mejorada de NTLM que proporciona un mecanismo Challenge-Response más robusto que NTLMv1, aunque sigue siendo una tecnología heredada.

**¿Dónde lo encuentro?**  
En sistemas Windows y entornos Active Directory donde aplicaciones o servicios todavía utilizan NTLM para autenticación.

**¿Por qué me afecta?**  
Aunque es más resistente que NTLMv1, puede seguir siendo objetivo de ataques como NTLM relay y captura de material de autenticación.

**¿Cómo se soluciona?**  
Reduciendo el uso de NTLM, priorizando Kerberos, aplicando protecciones contra relay y monitoreando autenticaciones NTLM anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede inducir o capturar una autenticación NTLMv2 y utilizar el material obtenido para ataques de relay o cracking offline.

## LM Hash

**¿Qué es?**  
LM Hash (LAN Manager Hash) es un método antiguo utilizado por Windows para almacenar representaciones de contraseñas, basado en un esquema criptográfico considerado extremadamente débil.

**¿Dónde lo encuentro?**  
En sistemas Windows antiguos que mantienen compatibilidad con LAN Manager, aunque los sistemas modernos normalmente no utilizan LM Hash para almacenar contraseñas.

**¿Por qué me afecta?**  
Su diseño permite ataques de cracking relativamente sencillos y representa un riesgo importante si todavía está habilitado o presente en un sistema.

**¿Cómo se soluciona?**  
Deshabilitando el almacenamiento de LM Hash, utilizando sistemas operativos compatibles con mecanismos modernos y eliminando dependencias de autenticación heredadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede obtener un LM Hash y utilizar herramientas de cracking para recuperar rápidamente partes de la contraseña original.

## NTLM Hash

**¿Qué es?**  
NTLM Hash es el hash MD4 de la contraseña codificada en UTF-16LE que Windows utiliza como representación de la contraseña en determinados mecanismos de autenticación NTLM.

**¿Dónde lo encuentro?**  
En bases de datos de credenciales de Windows y Active Directory, especialmente en componentes que almacenan los hashes asociados a las cuentas.

**¿Por qué me afecta?**  
El robo de un NTLM Hash puede permitir ataques offline y, en determinados escenarios, técnicas como Pass-the-Hash para autenticarse sin conocer la contraseña original.

**¿Cómo se soluciona?**  
Protegiendo las bases de datos de credenciales, aplicando mínimo privilegio, utilizando cuentas administradas cuando corresponda y reduciendo la dependencia de NTLM.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede extraer un NTLM Hash de un sistema comprometido y utilizarlo directamente en un ataque Pass-the-Hash o intentar recuperar la contraseña mediante cracking offline.
