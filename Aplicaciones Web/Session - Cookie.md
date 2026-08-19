
```markdown
## Session

**¿Qué es?**  
Mecanismo utilizado por una aplicación para mantener el estado de un usuario entre diferentes solicitudes, normalmente mediante un identificador de sesión asociado a información almacenada en el servidor.

**¿Dónde lo encuentro?**  
En aplicaciones web que requieren autenticación o mantienen información temporal del usuario, como sesiones iniciadas, carritos de compra o permisos.

**¿Por qué me afecta?**  
Una sesión mal protegida puede permitir secuestro de sesión, fijación de sesión o acceso no autorizado a cuentas y recursos.

**¿Cómo se soluciona?**  
Utilizar identificadores de sesión aleatorios, regenerarlos después de autenticarse, establecer tiempos de expiración y proteger su transmisión mediante HTTPS.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener o fijar un identificador de sesión válido para hacerse pasar por el usuario y acceder a los recursos disponibles durante esa sesión.

## Cookie

**¿Qué es?**  
Pequeño dato que un sitio web almacena en el navegador para conservar información entre solicitudes, como preferencias, identificadores de sesión o estados de autenticación.

**¿Dónde lo encuentro?**  
En el navegador del usuario y en las solicitudes HTTP enviadas posteriormente al dominio que estableció la cookie.

**¿Por qué me afecta?**  
Una cookie que contenga información sensible y esté mal configurada puede facilitar el robo de sesiones o la exposición de datos del usuario.

**¿Cómo se soluciona?**  
Configurar adecuadamente atributos como `Secure`, `HttpOnly` y `SameSite`, limitar su alcance y evitar almacenar información sensible directamente en ellas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar una cookie de sesión mediante ataques como XSS o interceptación de tráfico sin protección y utilizarla para suplantar al usuario.
```
