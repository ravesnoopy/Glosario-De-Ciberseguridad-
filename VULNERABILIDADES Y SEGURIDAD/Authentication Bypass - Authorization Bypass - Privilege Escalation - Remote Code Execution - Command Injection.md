# Authentication Bypass

**¿Qué es?**  
Authentication Bypass es una vulnerabilidad o técnica que permite a un atacante acceder a un sistema, aplicación o recurso sin completar correctamente el proceso de autenticación requerido.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, sistemas de autenticación, dispositivos de red y servicios que implementan mecanismos de inicio de sesión.

**¿Por qué me afecta?**  
Puede permitir que un atacante acceda directamente a cuentas, funciones o recursos protegidos sin disponer de credenciales válidas.

**¿Cómo se soluciona?**  
Validando la autenticación en el servidor, protegiendo correctamente las rutas y funciones sensibles y realizando pruebas de seguridad sobre los mecanismos de autenticación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar fallos en la lógica de autenticación, rutas protegidas o mecanismos de sesión que permitan acceder sin autenticarse correctamente.

---

# Authorization Bypass

**¿Qué es?**  
Authorization Bypass es una vulnerabilidad que permite a un usuario acceder a recursos o ejecutar acciones para las que no tiene permisos.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, sistemas empresariales, servicios cloud y sistemas que utilizan controles de acceso.

**¿Por qué me afecta?**  
Puede permitir que una cuenta con pocos privilegios acceda a información o funciones destinadas a usuarios con mayores permisos.

**¿Cómo se soluciona?**  
Validando la autorización en el servidor para cada recurso y acción, aplicando mínimo privilegio y realizando pruebas de control de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular solicitudes, identificadores de recursos o funciones para intentar acceder a información o acciones fuera de sus permisos.

---

# Privilege Escalation

**¿Qué es?**  
Privilege Escalation es el proceso mediante el cual un atacante obtiene permisos superiores a los que tenía originalmente.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, Active Directory, servicios cloud y entornos donde existen diferentes niveles de privilegios.

**¿Por qué me afecta?**  
Un atacante que comienza con acceso limitado puede utilizar una escalada de privilegios para obtener mayor control sobre sistemas o información.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, corrigiendo vulnerabilidades, restringiendo cuentas administrativas y monitoreando actividades relacionadas con cambios de privilegios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar vulnerabilidades, configuraciones incorrectas, permisos excesivos o credenciales privilegiadas para aumentar sus permisos.

---

# Remote Code Execution

**¿Qué es?**  
Remote Code Execution (RCE) es una vulnerabilidad que permite ejecutar código o comandos en un sistema objetivo desde una ubicación remota.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, servidores, servicios de red, frameworks y software vulnerable expuesto a redes.

**¿Por qué me afecta?**  
Una RCE puede permitir que un atacante tome control parcial o completo de un sistema afectado dependiendo de los privilegios disponibles.

**¿Cómo se soluciona?**  
Aplicando parches, validando correctamente las entradas, reduciendo privilegios y restringiendo la exposición de servicios vulnerables.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar una vulnerabilidad que permita controlar la ejecución de código para ejecutar acciones no autorizadas en el sistema afectado.

---

# Command Injection

**¿Qué es?**  
Command Injection es una vulnerabilidad que ocurre cuando una aplicación incorpora entradas controladas por un usuario en comandos del sistema sin aplicar una validación y separación adecuadas.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, scripts y servicios que ejecutan comandos del sistema operativo a partir de datos externos.

**¿Por qué me afecta?**  
Puede permitir que un atacante consiga que la aplicación ejecute comandos no autorizados con los privilegios del proceso vulnerable.

**¿Cómo se soluciona?**  
Evitando ejecutar comandos del sistema cuando exista una alternativa segura, utilizando APIs estructuradas, validando entradas y aplicando mínimo privilegio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular parámetros controlados por el usuario para intentar alterar la operación prevista por la aplicación y conseguir que se ejecuten comandos no autorizados.
