
## Session

**¿Qué es?**  
Session es el mecanismo mediante el cual una aplicación mantiene el estado y la identidad de un usuario mientras interactúa con ella durante un período determinado.

**¿Dónde lo encuentro?**  
En aplicaciones web, servidores de aplicaciones, APIs y sistemas que requieren mantener autenticado a un usuario entre diferentes solicitudes.

**¿Por qué me afecta?**  
Una sesión comprometida puede permitir que un atacante actúe como un usuario legítimo sin necesidad de conocer su contraseña.

**¿Cómo se soluciona?**  
Utilizando identificadores de sesión aleatorios, expiración adecuada, regeneración después de autenticarse y protección mediante HTTPS.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar, fijar o reutilizar un identificador de sesión válido para hacerse pasar por otro usuario.

## Cookie

**¿Qué es?**  
Cookie es un pequeño dato almacenado por el navegador que permite a un sitio web conservar información entre diferentes solicitudes.

**¿Dónde lo encuentro?**  
En navegadores web y aplicaciones que utilizan cookies para sesiones, preferencias, autenticación u otras funciones.

**¿Por qué me afecta?**  
Una cookie de autenticación comprometida puede permitir el acceso a una cuenta sin necesidad de introducir nuevamente las credenciales.

**¿Cómo se soluciona?**  
Protegiendo las cookies sensibles con atributos como `Secure`, `HttpOnly` y `SameSite`, además de utilizar HTTPS y gestionar correctamente su expiración.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar una cookie de sesión mediante ataques como XSS o interceptación de comunicaciones para reutilizarla y acceder a la cuenta de la víctima.
