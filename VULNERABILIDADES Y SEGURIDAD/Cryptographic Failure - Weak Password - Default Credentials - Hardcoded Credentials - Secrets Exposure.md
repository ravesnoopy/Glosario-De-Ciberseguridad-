# Cryptographic Failure

**¿Qué es?**  
Cryptographic Failure es una debilidad que ocurre cuando los mecanismos criptográficos utilizados para proteger información son inexistentes, incorrectos, débiles o están mal implementados.

**¿Dónde lo encuentro?**  
En aplicaciones, APIs, bases de datos, sistemas de autenticación, comunicaciones de red y almacenamiento de información sensible.

**¿Por qué me afecta?**  
Puede permitir que información confidencial, credenciales o datos sensibles sean expuestos, modificados o recuperados por personas no autorizadas.

**¿Cómo se soluciona?**  
Utilizando algoritmos criptográficos actuales y adecuados, protegiendo correctamente las claves y evitando protocolos o configuraciones criptográficas obsoletas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar información protegida con algoritmos débiles, configuraciones inseguras o implementaciones incorrectas para intentar recuperar datos protegidos.

---

# Weak Password

**¿Qué es?**  
Weak Password es una contraseña que resulta fácil de adivinar, descubrir o romper debido a su poca longitud, simplicidad, reutilización o predictibilidad.

**¿Dónde lo encuentro?**  
En cuentas de usuarios, cuentas administrativas, servicios, aplicaciones, dispositivos de red y sistemas empresariales.

**¿Por qué me afecta?**  
Una contraseña débil puede permitir el acceso no autorizado a cuentas y convertirse en un punto de entrada para comprometer otros sistemas.

**¿Cómo se soluciona?**  
Utilizando contraseñas largas y únicas, gestores de contraseñas, MFA y políticas que eviten credenciales comunes o comprometidas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar adivinar o probar contraseñas comunes y credenciales previamente expuestas para obtener acceso a una cuenta.

---

# Default Credentials

**¿Qué es?**  
Default Credentials son credenciales proporcionadas originalmente por el fabricante o proveedor de un sistema, aplicación o dispositivo.

**¿Dónde lo encuentro?**  
En dispositivos de red, aplicaciones, cámaras, servidores, sistemas empresariales y software instalado recientemente.

**¿Por qué me afecta?**  
Si las credenciales predeterminadas permanecen activas, cualquier persona que las conozca podría utilizarlas para obtener acceso no autorizado.

**¿Cómo se soluciona?**  
Cambiando las credenciales predeterminadas antes de poner el sistema en producción y aplicando políticas de autenticación seguras.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede probar credenciales conocidas del fabricante contra sistemas que todavía utilicen la configuración predeterminada.

---

# Hardcoded Credentials

**¿Qué es?**  
Hardcoded Credentials son credenciales incorporadas directamente dentro del código fuente, archivos de configuración o componentes de una aplicación.

**¿Dónde lo encuentro?**  
En código fuente, scripts, aplicaciones, archivos de configuración, repositorios y software desplegado.

**¿Por qué me afecta?**  
Si las credenciales quedan expuestas, un atacante puede recuperarlas y utilizarlas para acceder a sistemas, servicios o datos.

**¿Cómo se soluciona?**  
Eliminando credenciales del código, utilizando gestores de secretos, variables de entorno protegidas y mecanismos seguros de rotación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede analizar código, archivos o repositorios para localizar credenciales incorporadas y utilizarlas para obtener acceso a recursos asociados.

---

# Secrets Exposure

**¿Qué es?**  
Secrets Exposure es la exposición accidental o no autorizada de información sensible utilizada para autenticar o acceder a servicios, como API keys, tokens, contraseñas o claves privadas.

**¿Dónde lo encuentro?**  
En repositorios de código, archivos de configuración, logs, scripts, aplicaciones, servicios cloud y sistemas de almacenamiento.

**¿Por qué me afecta?**  
Un secreto expuesto puede proporcionar acceso directo a servicios, cuentas, APIs o infraestructura sin necesidad de comprometer primero otro mecanismo de autenticación.

**¿Cómo se soluciona?**  
Utilizando gestores de secretos, evitando almacenar secretos en código o logs, aplicando rotación y revocando inmediatamente los secretos que hayan sido expuestos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar secretos expuestos en repositorios, archivos, logs o configuraciones y utilizarlos para acceder a los recursos que protegen.
