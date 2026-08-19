
## IAM

**¿Qué es?**  
Identity and Access Management es el conjunto de mecanismos utilizados para administrar identidades y controlar qué usuarios, aplicaciones o servicios pueden acceder a determinados recursos.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones empresariales, servicios cloud, APIs y plataformas que requieren autenticación y autorización.

**¿Por qué me afecta?**  
Una configuración incorrecta de IAM puede generar privilegios excesivos, accesos no autorizados y facilitar el movimiento lateral o la escalada de privilegios.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, utilizar MFA, revisar permisos periódicamente, eliminar identidades innecesarias y monitorear actividades de autenticación y autorización.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer una identidad o explotar permisos excesivos para acceder a recursos adicionales y ampliar su control.


## Identity

**¿Qué es?**  
Representación de una persona, aplicación, servicio o dispositivo que permite al sistema determinar quién o qué está realizando una acción.

**¿Dónde lo encuentro?**  
En sistemas de autenticación, directorios, plataformas cloud, aplicaciones, APIs y sistemas de gestión de acceso.

**¿Por qué me afecta?**  
El compromiso de una identidad puede proporcionar al atacante los permisos asociados a ella sin necesidad de comprometer directamente cada recurso.

**¿Cómo se soluciona?**  
Utilizar autenticación robusta, MFA, mínimo privilegio, gestión adecuada del ciclo de vida de las cuentas y monitoreo de actividades.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer una identidad mediante credenciales robadas, phishing, tokens expuestos u otras técnicas para actuar como un usuario legítimo.


## Role

**¿Qué es?**  
Conjunto de permisos que puede ser asumido o asignado a una identidad para definir qué acciones puede realizar sobre determinados recursos.

**¿Dónde lo encuentro?**  
En plataformas cloud, sistemas IAM, aplicaciones empresariales y sistemas de autorización basados en roles.

**¿Por qué me afecta?**  
Un rol demasiado permisivo puede conceder capacidades administrativas o acceso a información que una identidad no debería tener.

**¿Cómo se soluciona?**  
Diseñar roles específicos, aplicar mínimo privilegio, revisar asignaciones periódicamente y eliminar permisos innecesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Si compromete una identidad capaz de asumir un rol privilegiado, podría utilizarlo para obtener permisos adicionales y ampliar su acceso.


## Permission

**¿Qué es?**  
Autorización específica que determina qué acción puede realizar una identidad sobre un recurso, como leer, modificar, eliminar o ejecutar.

**¿Dónde lo encuentro?**  
En sistemas IAM, aplicaciones, sistemas operativos, bases de datos, APIs y servicios cloud.

**¿Por qué me afecta?**  
Permisos excesivos pueden permitir que una cuenta comprometida realice acciones de mayor impacto del necesario.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, conceder únicamente las acciones necesarias y revisar periódicamente los permisos efectivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría una identidad comprometida con permisos excesivos para acceder a información, modificar recursos o realizar acciones administrativas.


## Policy

**¿Qué es?**  
Regla o conjunto de reglas que define qué acciones están permitidas o denegadas para determinadas identidades y recursos.

**¿Dónde lo encuentro?**  
En sistemas IAM, servicios cloud, APIs y plataformas que utilizan políticas para controlar el acceso.

**¿Por qué me afecta?**  
Una política mal configurada puede conceder acceso público, permisos administrativos o acceso a recursos que deberían estar restringidos.

**¿Cómo se soluciona?**  
Utilizar políticas específicas y restrictivas, evitar permisos amplios innecesarios, revisar cambios y aplicar el principio de mínimo privilegio.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría políticas permisivas o configuraciones incorrectas que le permitan realizar acciones fuera de los privilegios previstos.


## Access Key

**¿Qué es?**  
Credencial utilizada por una aplicación, usuario o servicio para autenticarse ante determinados servicios, especialmente APIs cloud.

**¿Dónde lo encuentro?**  
En aplicaciones, scripts, herramientas de administración, configuraciones y sistemas que realizan solicitudes autenticadas a servicios cloud.

**¿Por qué me afecta?**  
Una access key expuesta puede permitir que un atacante se autentique como la identidad asociada y utilice los permisos disponibles.

**¿Cómo se soluciona?**  
Evitar almacenarlas en código, utilizar mecanismos temporales cuando sea posible, protegerlas mediante gestores de secretos y rotarlas o revocarlas si se exponen.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría claves expuestas en repositorios, archivos o sistemas comprometidos para utilizarlas contra los servicios a los que proporcionan acceso.


## Secret Key

**¿Qué es?**  
Credencial secreta asociada a determinados mecanismos de autenticación, utilizada junto con otros identificadores para demostrar que una solicitud proviene de una identidad autorizada.

**¿Dónde lo encuentro?**  
En aplicaciones, herramientas, configuraciones y sistemas que utilizan credenciales para firmar o autenticar solicitudes ante servicios.

**¿Por qué me afecta?**  
Su exposición puede permitir que un atacante genere solicitudes autenticadas o suplante la identidad asociada, dependiendo del mecanismo utilizado.

**¿Cómo se soluciona?**  
Almacenarla mediante gestores de secretos, evitar incluirla en código o repositorios, limitar su uso y rotarla o revocarla inmediatamente ante una exposición.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría obtener la clave mediante filtraciones, repositorios, archivos de configuración o sistemas comprometidos para utilizarla junto con la identidad correspondiente.
