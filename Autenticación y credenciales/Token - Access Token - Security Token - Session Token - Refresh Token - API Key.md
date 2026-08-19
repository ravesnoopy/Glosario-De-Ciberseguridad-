
## Token

**¿Qué es?**  
Elemento de información utilizado para representar una identidad, sesión, autorización o permiso dentro de un sistema sin necesidad de enviar continuamente las credenciales originales.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, sistemas de autenticación, aplicaciones móviles, servicios en la nube y mecanismos de gestión de sesiones.

**¿Por qué me afecta?**  
Si un token es robado, manipulado o utilizado durante más tiempo del necesario, puede permitir acceso no autorizado a los recursos asociados.

**¿Cómo se soluciona?**  
Proteger los tokens, limitar su duración y privilegios, transmitirlos mediante canales seguros y revocarlos cuando exista sospecha de compromiso.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría obtener un token válido mediante robo de sesión, malware, exposición accidental u otra técnica para utilizarlo como credencial.


## Access Token

**¿Qué es?**  
Credencial que representa la autorización de una identidad para acceder a determinados recursos o servicios durante un periodo y alcance definidos.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, servicios cloud y sistemas de autorización como OAuth 2.0.

**¿Por qué me afecta?**  
Su compromiso puede permitir acceder directamente a los recursos y operaciones incluidos en sus permisos.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, limitar duración y alcance, proteger el almacenamiento del token y utilizar canales seguros para su transmisión.

**¿Cómo lo usaría un atacante en mi contra?**  
Si obtiene un access token válido, podría utilizarlo para realizar solicitudes a los recursos permitidos haciéndose pasar por la identidad autorizada.


## Security Token

**¿Qué es?**  
Credencial o artefacto utilizado por un sistema para representar información de seguridad, como una identidad, autenticación o autorización.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, servicios de autenticación, APIs y mecanismos de control de acceso.

**¿Por qué me afecta?**  
Un security token comprometido puede permitir la suplantación de una identidad o el acceso a recursos según los privilegios que represente.

**¿Cómo se soluciona?**  
Proteger los mecanismos de autenticación, aplicar mínimo privilegio, controlar la vida útil de las credenciales y monitorear su uso anómalo.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría obtener o abusar de un token de seguridad para actuar con los permisos asociados a otra identidad.


## Session Token

**¿Qué es?**  
Valor que identifica una sesión autenticada y permite a una aplicación reconocer las solicitudes posteriores como pertenecientes a ese usuario.

**¿Dónde lo encuentro?**  
En aplicaciones web y APIs, normalmente asociado a cookies, cabeceras u otros mecanismos utilizados para mantener sesiones.

**¿Por qué me afecta?**  
El robo de un session token puede permitir secuestrar una sesión activa sin necesidad de conocer la contraseña del usuario.

**¿Cómo se soluciona?**  
Utilizar HTTPS, tokens impredecibles y de corta duración, regenerarlos después de eventos importantes de autenticación y proteger cookies con atributos como `HttpOnly`, `Secure` y `SameSite`.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría obtener el token de sesión de una víctima y reutilizarlo para acceder a la aplicación como si fuera el usuario legítimo.


## Refresh Token

**¿Qué es?**  
Credencial utilizada para obtener nuevos access tokens cuando estos expiran, evitando que el usuario tenga que autenticarse nuevamente.

**¿Dónde lo encuentro?**  
En sistemas de autenticación y autorización modernos, especialmente en aplicaciones que utilizan OAuth 2.0 u otros mecanismos basados en tokens de corta duración.

**¿Por qué me afecta?**  
Su compromiso puede proporcionar acceso prolongado porque permite generar nuevos access tokens mientras el refresh token siga siendo válido.

**¿Cómo se soluciona?**  
Almacenarlo de forma segura, limitar su duración, aplicar rotación y revocación, y detectar su reutilización sospechosa.

**¿Cómo lo usaría un atacante en mi contra?**  
Si obtiene un refresh token válido, podría intentar utilizarlo para conseguir nuevos access tokens y mantener acceso a los recursos autorizados.


## API Key

**¿Qué es?**  
Credencial utilizada por una aplicación o cliente para identificarse o autorizar solicitudes hacia una API o servicio.

**¿Dónde lo encuentro?**  
En aplicaciones, integraciones, scripts, archivos de configuración, variables de entorno y servicios que requieren autenticación mediante claves.

**¿Por qué me afecta?**  
Una API Key expuesta puede permitir que terceros utilicen servicios, consulten información o consuman recursos bajo los permisos asociados a esa clave.

**¿Cómo se soluciona?**  
No incluir claves en código público, almacenarlas mediante gestores de secretos o mecanismos seguros, limitar sus permisos y rotarlas o revocarlas cuando se comprometan.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría API Keys expuestas en código, repositorios, archivos o registros para utilizarlas contra el servicio al que proporcionan acceso.
