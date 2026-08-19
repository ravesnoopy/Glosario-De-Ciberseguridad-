
## Authentication

**¿Qué es?**  
Authentication es el proceso mediante el cual un sistema verifica la identidad de un usuario, dispositivo o servicio antes de permitirle acceder.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, APIs, VPN, servicios cloud y cualquier sistema que requiera verificar la identidad de quien solicita acceso.

**¿Por qué me afecta?**  
Una autenticación débil puede permitir que un atacante acceda a cuentas y recursos utilizando credenciales robadas, adivinadas o comprometidas.

**¿Cómo se soluciona?**  
Utilizando contraseñas resistentes, MFA, controles contra intentos automatizados y mecanismos de autenticación adecuados al nivel de riesgo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar o adivinar credenciales mediante phishing, fuerza bruta, password spraying o credential stuffing para hacerse pasar por un usuario legítimo.

## Authorization

**¿Qué es?**  
Authorization es el proceso mediante el cual un sistema determina qué recursos o acciones puede utilizar un usuario después de ser autenticado.

**¿Dónde lo encuentro?**  
En aplicaciones, APIs, sistemas operativos, bases de datos, servicios cloud y sistemas que utilizan roles o permisos.

**¿Por qué me afecta?**  
Una autorización incorrecta puede permitir que un usuario acceda a información o realice acciones que exceden sus permisos.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, controles de acceso adecuados y verificando los permisos en el servidor para cada solicitud.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar fallos de autorización para acceder a recursos de otros usuarios o ejecutar funciones administrativas sin los permisos correspondientes.

## Accountability

**¿Qué es?**  
Accountability es la capacidad de atribuir acciones realizadas sobre sistemas o recursos a una identidad o entidad responsable mediante controles y registros.

**¿Dónde lo encuentro?**  
En registros de auditoría, sistemas de autenticación, SIEM, aplicaciones, sistemas operativos y plataformas que registran actividades de usuarios y administradores.

**¿Por qué me afecta?**  
Sin trazabilidad adecuada es más difícil detectar incidentes, investigar actividades maliciosas y determinar quién realizó una acción.

**¿Cómo se soluciona?**  
Utilizando cuentas individuales, registros de auditoría, sincronización de tiempo, monitoreo centralizado y controles que eviten compartir credenciales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar cuentas compartidas, credenciales robadas o mecanismos para alterar o eliminar registros con el objetivo de dificultar la atribución de sus acciones.

## Non-repudiation

**¿Qué es?**  
Non-repudiation es la propiedad de seguridad que proporciona evidencia suficiente para demostrar que una determinada entidad realizó una acción o transacción.

**¿Dónde lo encuentro?**  
En firmas digitales, registros de auditoría protegidos, certificados y sistemas que requieren evidencia verificable de determinadas operaciones.

**¿Por qué me afecta?**  
Ayuda a demostrar la autenticidad e integridad de acciones importantes y dificulta negar posteriormente una operación realizada.

**¿Cómo se soluciona?**  
Utilizando firmas digitales, controles de integridad, registros protegidos y mecanismos de auditoría confiables.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer claves privadas, manipular registros o utilizar identidades comprometidas para realizar acciones cuya atribución resulte difícil de verificar.

## Least Privilege

**¿Qué es?**  
Least Privilege es el principio de otorgar a cada usuario, proceso o servicio únicamente los permisos necesarios para realizar sus funciones.

**¿Dónde lo encuentro?**  
En cuentas de usuario, roles, aplicaciones, servicios, sistemas operativos, bases de datos, entornos cloud y controles de acceso.

**¿Por qué me afecta?**  
Limita el impacto de una cuenta o sistema comprometido al reducir las acciones y recursos que un atacante puede utilizar.

**¿Cómo se soluciona?**  
Revisando permisos periódicamente, eliminando privilegios innecesarios, utilizando roles adecuados y separando cuentas administrativas de las cuentas normales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una cuenta con permisos excesivos para acceder a recursos adicionales, modificar sistemas o escalar su control dentro del entorno.

## Defense in Depth

**¿Qué es?**  
Defense in Depth es una estrategia de seguridad que utiliza múltiples capas de controles para proteger los sistemas, de modo que el fallo de una medida no implique automáticamente el compromiso del entorno.

**¿Dónde lo encuentro?**  
En arquitecturas que combinan controles como MFA, firewalls, segmentación, cifrado, EDR, SIEM, controles de acceso y respaldos.

**¿Por qué me afecta?**  
Reduce la probabilidad de que una única vulnerabilidad o control fallido permita a un atacante comprometer completamente un sistema o red.

**¿Cómo se soluciona?**  
Implementando controles preventivos, detectivos y de respuesta en diferentes capas de la infraestructura y revisando periódicamente su efectividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evadir cada capa de seguridad progresivamente, buscando una combinación de debilidades que le permita avanzar hacia sus objetivos.
