
## Privileged Account

**¿Qué es?**  
Una Privileged Account es una cuenta con permisos elevados que puede realizar acciones administrativas o acceder a recursos críticos dentro de un sistema o entorno.

**¿Dónde lo encuentro?**  
En sistemas operativos, Active Directory, bases de datos, servidores, aplicaciones empresariales, dispositivos de red y plataformas cloud.

**¿Por qué me afecta?**  
Si una cuenta privilegiada es comprometida, un atacante puede obtener un nivel de acceso suficiente para modificar configuraciones, acceder a información sensible o controlar sistemas críticos.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, MFA, separación de cuentas administrativas y monitoreo de actividades privilegiadas, además de evitar el uso de cuentas administrativas para tareas cotidianas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una cuenta privilegiada mediante phishing, robo de credenciales, explotación de vulnerabilidades o escalación de privilegios para obtener control sobre sistemas críticos.

## Credential Rotation

**¿Qué es?**  
Credential Rotation es el proceso de cambiar periódicamente contraseñas, claves, tokens u otras credenciales para reducir el riesgo asociado con credenciales expuestas o comprometidas.

**¿Dónde lo encuentro?**  
En cuentas administrativas, cuentas de servicio, aplicaciones, bases de datos, APIs, dispositivos de red y plataformas cloud.

**¿Por qué me afecta?**  
Si una credencial permanece válida durante mucho tiempo después de haber sido comprometida, un atacante puede mantener o recuperar acceso a los sistemas.

**¿Cómo se soluciona?**  
Estableciendo procesos automáticos de rotación cuando sea posible, utilizando credenciales administradas y evitando reutilizar secretos antiguos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar una credencial robada mientras siga siendo válida para mantener acceso a sistemas o servicios comprometidos.

## Credential Revocation

**¿Qué es?**  
Credential Revocation es el proceso de invalidar una credencial para impedir que continúe siendo utilizada para autenticarse o acceder a recursos.

**¿Dónde lo encuentro?**  
En cuentas de usuario, tokens de acceso, certificados, claves API, sesiones y otros mecanismos utilizados para controlar el acceso.

**¿Por qué me afecta?**  
Revocar rápidamente una credencial comprometida puede impedir que un atacante continúe utilizando el acceso obtenido.

**¿Cómo se soluciona?**  
Deshabilitando cuentas comprometidas, invalidando tokens y sesiones, revocando certificados o claves y verificando que el acceso haya sido eliminado de todos los sistemas relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar una credencial comprometida antes de que sea revocada para mantener acceso, acceder a recursos adicionales o establecer mecanismos de persistencia.
