
## Kerberos

**¿Qué es?**  
Protocolo de autenticación basado en tickets que permite a usuarios y servicios demostrar su identidad dentro de una red sin enviar directamente la contraseña a cada servicio.

**¿Dónde lo encuentro?**  
Principalmente en entornos Windows con Active Directory, donde se utiliza como uno de los mecanismos principales de autenticación entre usuarios, equipos y servicios.

**¿Por qué me afecta?**  
Kerberos es fundamental para la autenticación empresarial, pero sus tickets, cuentas y configuraciones pueden ser abusados para técnicas como Pass-the-Ticket, Kerberoasting o Golden Ticket.

**¿Cómo se soluciona?**  
Mantener Active Directory actualizado, proteger cuentas privilegiadas, utilizar contraseñas robustas, aplicar mínimo privilegio y monitorear solicitudes y usos anómalos de tickets Kerberos.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras comprometer una cuenta o sistema, podría intentar obtener, robar o manipular tickets Kerberos para autenticarse y ampliar su acceso dentro del dominio.


## Ticket

**¿Qué es?**  
Credencial temporal emitida por Kerberos que permite a una identidad autenticarse ante determinados servicios sin tener que proporcionar nuevamente su contraseña.

**¿Dónde lo encuentro?**  
En sistemas y sesiones que utilizan Kerberos, especialmente en entornos Active Directory donde los usuarios y equipos mantienen tickets durante sus sesiones.

**¿Por qué me afecta?**  
Un ticket comprometido puede permitir que un atacante se haga pasar por la identidad asociada durante el periodo en que sea válido y tenga los permisos correspondientes.

**¿Cómo se soluciona?**  
Proteger los sistemas donde se almacenan tickets, limitar privilegios, controlar la duración de las credenciales y monitorear comportamientos anómalos de autenticación Kerberos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría obtener un ticket válido de una sesión comprometida y reutilizarlo para acceder a los servicios autorizados para esa identidad.


## TGT

**¿Qué es?**  
Ticket Granting Ticket es un ticket de Kerberos emitido por el KDC que permite a un usuario solicitar posteriormente tickets de servicio sin volver a realizar una autenticación completa.

**¿Dónde lo encuentro?**  
En sesiones autenticadas mediante Kerberos dentro de Active Directory, donde el TGT se utiliza como credencial para solicitar otros tickets.

**¿Por qué me afecta?**  
El compromiso de un TGT puede permitir al atacante solicitar tickets de servicio en nombre de la identidad asociada y ampliar su acceso.

**¿Cómo se soluciona?**  
Proteger las credenciales que permiten obtener TGT, aplicar mínimo privilegio, proteger cuentas privilegiadas y monitorear solicitudes y comportamientos anómalos de Kerberos.

**¿Cómo lo usaría un atacante en mi contra?**  
Si obtiene un TGT válido, podría intentar reutilizarlo para solicitar TGS y acceder a servicios con los privilegios de la identidad comprometida.


## TGS

**¿Qué es?**  
Ticket Granting Service es el ticket emitido para permitir que una identidad autenticada acceda a un servicio específico dentro de un entorno Kerberos.

**¿Dónde lo encuentro?**  
En entornos Active Directory cuando un usuario o equipo solicita acceso a servicios identificados mediante nombres principales de servicio.

**¿Por qué me afecta?**  
Los TGS pueden contener material que, en determinados escenarios, puede ser utilizado para ataques como Kerberoasting contra cuentas de servicio vulnerables.

**¿Cómo se soluciona?**  
Proteger las cuentas de servicio con contraseñas robustas, aplicar mínimo privilegio, utilizar cuentas administradas cuando sea posible y monitorear solicitudes de tickets anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría solicitar TGS asociados a servicios para intentar obtener material de autenticación y posteriormente atacar offline las credenciales de cuentas de servicio vulnerables.


## Service Principal Name

**¿Qué es?**  
Identificador utilizado por Kerberos para asociar una instancia de servicio con la cuenta de dominio que ejecuta dicho servicio.

**¿Dónde lo encuentro?**  
En Active Directory, asociado a cuentas de usuario, equipos y servicios que requieren autenticación mediante Kerberos.

**¿Por qué me afecta?**  
Los SPN permiten identificar servicios Kerberos y pueden revelar cuentas de servicio susceptibles a técnicas como Kerberoasting si están configuradas de forma insegura.

**¿Cómo se soluciona?**  
Mantener únicamente los SPN necesarios, utilizar cuentas de servicio administradas cuando sea posible, aplicar mínimo privilegio y proteger adecuadamente sus credenciales.

**¿Cómo lo usaría un atacante en mi contra?**  
Enumeraría SPN para identificar servicios asociados a cuentas de dominio y buscar oportunidades para obtener material de autenticación de cuentas de servicio vulnerables.


## SPN

**¿Qué es?**  
Service Principal Name es la forma abreviada de `Service Principal Name` y representa el identificador único utilizado por Kerberos para localizar una instancia de servicio asociada a una cuenta.

**¿Dónde lo encuentro?**  
En objetos de Active Directory correspondientes a equipos y cuentas que ejecutan servicios autenticados mediante Kerberos.

**¿Por qué me afecta?**  
Una configuración incorrecta de SPN puede facilitar la identificación de cuentas de servicio y ser aprovechada en ataques contra sus credenciales.

**¿Cómo se soluciona?**  
Revisar periódicamente los SPN registrados, eliminar asociaciones innecesarias y asegurar que las cuentas asociadas utilicen credenciales robustas y privilegios mínimos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría enumerar los SPN del dominio para identificar servicios y cuentas que podrían ser objetivos de técnicas de abuso de Kerberos.


## KDC

**¿Qué es?**  
Key Distribution Center es el componente central de Kerberos encargado de gestionar la autenticación y emisión de tickets. En Active Directory, sus funciones son proporcionadas por los controladores de dominio.

**¿Dónde lo encuentro?**  
En entornos que utilizan Kerberos, especialmente en dominios Windows donde los controladores de dominio actúan como KDC.

**¿Por qué me afecta?**  
El KDC es un componente crítico de la infraestructura de autenticación; su compromiso puede tener un impacto amplio sobre la seguridad del dominio.

**¿Cómo se soluciona?**  
Proteger los controladores de dominio, restringir el acceso administrativo, aplicar actualizaciones, utilizar cuentas privilegiadas de forma controlada y monitorear eventos de autenticación Kerberos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer cuentas o componentes relacionados con el KDC para obtener capacidades que le permitan abusar de la autenticación y ampliar el control sobre el dominio.
