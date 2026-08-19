
## File Upload

**¿Qué es?**  
File Upload es la funcionalidad que permite a un usuario enviar archivos a una aplicación o servidor. Si no está correctamente controlada, puede convertirse en un punto de entrada para archivos maliciosos.

**¿Dónde lo encuentro?**  
En formularios web, perfiles de usuario, sistemas de documentos, plataformas de gestión de archivos y aplicaciones que permiten adjuntar contenido.

**¿Por qué me afecta?**  
Una implementación insegura puede permitir la carga de archivos ejecutables o maliciosos, sobrescribir archivos o comprometer el servidor.

**¿Cómo se soluciona?**  
Validando tipo, extensión y tamaño, utilizando listas permitidas, almacenando los archivos fuera de directorios ejecutables y aplicando controles de acceso adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar cargar un archivo malicioso para ejecutar código, instalar una Web Shell o aprovechar la forma en que la aplicación procesa los archivos.

## Directory Listing

**¿Qué es?**  
Directory Listing es una función del servidor web que muestra el contenido de un directorio cuando no existe un archivo de índice configurado.

**¿Dónde lo encuentro?**  
En servidores web donde el listado de directorios está habilitado, especialmente cuando una URL apunta directamente a una carpeta sin una página predeterminada.

**¿Por qué me afecta?**  
Puede revelar nombres de archivos, directorios, copias de seguridad, configuraciones u otra información que ayude a identificar recursos sensibles.

**¿Cómo se soluciona?**  
Deshabilitando el listado de directorios y restringiendo el acceso a archivos y carpetas que no deban estar disponibles públicamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar los archivos expuestos para descubrir información útil, identificar posibles objetivos o localizar archivos sensibles.

## IDOR

**¿Qué es?**  
IDOR (Insecure Direct Object Reference) es una vulnerabilidad que ocurre cuando una aplicación utiliza referencias a objetos, como identificadores, sin verificar correctamente si el usuario tiene permiso para acceder a ellos.

**¿Dónde lo encuentro?**  
En aplicaciones web y APIs que utilizan identificadores de usuarios, documentos, cuentas, pedidos u otros recursos en parámetros o rutas.

**¿Por qué me afecta?**  
Puede permitir que un usuario acceda, modifique o elimine recursos pertenecientes a otros usuarios sin autorización.

**¿Cómo se soluciona?**  
Implementando comprobaciones de autorización en el servidor para cada recurso solicitado y evitando confiar únicamente en identificadores proporcionados por el cliente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar un identificador en una solicitud para intentar acceder a información o recursos que pertenecen a otro usuario.

## Session Hijacking

**¿Qué es?**  
Session Hijacking es el robo o apropiación de una sesión autenticada para actuar como la víctima sin necesidad de conocer directamente sus credenciales.

**¿Dónde lo encuentro?**  
En aplicaciones web que utilizan cookies, tokens u otros identificadores para mantener sesiones autenticadas.

**¿Por qué me afecta?**  
Si un atacante obtiene un identificador de sesión válido, puede acceder a la cuenta y realizar acciones con los permisos de la víctima.

**¿Cómo se soluciona?**  
Utilizando HTTPS, cookies con atributos `Secure`, `HttpOnly` y `SameSite`, expiración adecuada de sesiones, rotación de identificadores y protección contra XSS.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede robar un identificador de sesión mediante malware, phishing, XSS u otras técnicas y utilizarlo para hacerse pasar por la víctima.

## Credential Stuffing

**¿Qué es?**  
Credential Stuffing es un ataque que utiliza combinaciones de usuario y contraseña obtenidas de filtraciones anteriores para intentar acceder a otras cuentas.

**¿Dónde lo encuentro?**  
En servicios web, aplicaciones, APIs y plataformas donde los usuarios reutilizan credenciales entre diferentes servicios.

**¿Por qué me afecta?**  
La reutilización de contraseñas permite que una filtración en un servicio comprometa cuentas de la víctima en otros sistemas.

**¿Cómo se soluciona?**  
Utilizando contraseñas únicas, MFA, detección de patrones de inicio de sesión anómalos, protección contra automatización y bloqueo de credenciales comprometidas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede automatizar intentos de inicio de sesión utilizando listas de credenciales filtradas hasta encontrar cuentas que utilicen las mismas contraseñas.

## Brute Force

**¿Qué es?**  
Brute Force es un ataque que intenta obtener una credencial probando repetidamente diferentes contraseñas o combinaciones hasta encontrar una válida.

**¿Dónde lo encuentro?**  
En servicios de autenticación como aplicaciones web, VPN, SSH, RDP, APIs y otros sistemas protegidos mediante credenciales.

**¿Por qué me afecta?**  
Una política de contraseñas débil y la ausencia de controles contra intentos repetidos pueden facilitar el acceso no autorizado a una cuenta.

**¿Cómo se soluciona?**  
Implementando MFA, límites de intentos, bloqueo o retrasos progresivos, contraseñas resistentes y mecanismos de detección de intentos automatizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar numerosos intentos de autenticación contra una cuenta o servicio hasta descubrir una contraseña válida.
