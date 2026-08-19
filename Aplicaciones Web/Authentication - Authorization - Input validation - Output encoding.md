
## Authentication

**¿Qué es?**  
Authentication es el proceso mediante el cual un sistema verifica la identidad de un usuario, dispositivo o servicio antes de permitirle acceder.

**¿Dónde lo encuentro?**  
En formularios de inicio de sesión, aplicaciones web, VPN, sistemas operativos, APIs y servicios que requieren verificar la identidad de sus usuarios.

**¿Por qué me afecta?**  
Una autenticación débil puede permitir accesos no autorizados, robo de cuentas y compromiso de información o recursos protegidos.

**¿Cómo se soluciona?**  
Utilizando contraseñas robustas, MFA, almacenamiento seguro de credenciales, mecanismos de bloqueo y protocolos de autenticación adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar, adivinar o reutilizar credenciales mediante phishing, credential stuffing, password spraying u otros ataques para acceder a una cuenta.

## Authorization

**¿Qué es?**  
Authorization es el proceso que determina qué recursos o acciones puede utilizar un usuario después de haber sido autenticado.

**¿Dónde lo encuentro?**  
En aplicaciones, APIs, sistemas operativos, bases de datos y servicios que asignan permisos o roles a usuarios y cuentas.

**¿Por qué me afecta?**  
Una autorización incorrecta puede permitir que un usuario acceda a información o funciones que no debería poder utilizar.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, controles de acceso basados en roles o atributos y verificando los permisos en cada solicitud a recursos protegidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar fallos de autorización para acceder a recursos de otros usuarios, elevar sus privilegios o ejecutar acciones restringidas.

## Input validation

**¿Qué es?**  
Input validation es el proceso de comprobar que los datos proporcionados por un usuario o sistema cumplen con el formato, tipo, longitud y valores esperados antes de ser procesados.

**¿Dónde lo encuentro?**  
En formularios web, APIs, aplicaciones, scripts y cualquier componente que reciba datos externos antes de procesarlos o almacenarlos.

**¿Por qué me afecta?**  
Una validación deficiente puede permitir que entradas maliciosas lleguen a componentes sensibles y faciliten ataques como inyección SQL, command injection o XSS.

**¿Cómo se soluciona?**  
Validando los datos mediante reglas estrictas, listas permitidas cuando sea posible y controles tanto del lado del servidor como del cliente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enviar datos manipulados o inesperados para evadir controles y provocar la ejecución de comandos, consultas o código no autorizado.

## Output encoding

**¿Qué es?**  
Output encoding es la transformación de datos antes de mostrarlos o enviarlos a otro contexto para evitar que caracteres especiales sean interpretados como código.

**¿Dónde lo encuentro?**  
En aplicaciones web que muestran datos proporcionados por usuarios dentro de HTML, JavaScript, URLs, CSS u otros contextos donde el contenido puede ser interpretado.

**¿Por qué me afecta?**  
Una codificación de salida incorrecta puede permitir ataques como Cross-Site Scripting (XSS), haciendo que contenido controlado por un atacante sea interpretado como código.

**¿Cómo se soluciona?**  
Aplicando la codificación adecuada según el contexto donde se inserta el dato y utilizando mecanismos seguros de renderizado proporcionados por el framework.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede introducir contenido especialmente diseñado para que, al ser mostrado por la aplicación, el navegador lo interprete como código y ejecute acciones en el contexto de la víctima.
