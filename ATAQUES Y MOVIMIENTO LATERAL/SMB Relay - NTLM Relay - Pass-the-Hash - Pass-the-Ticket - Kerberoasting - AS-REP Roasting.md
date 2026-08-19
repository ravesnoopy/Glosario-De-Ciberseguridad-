
## SMB Relay

**¿Qué es?**  
Técnica de ataque que aprovecha la autenticación NTLM para reenviar las credenciales o autenticación de una víctima hacia otro servicio SMB, intentando autenticarse sin conocer directamente su contraseña.

**¿Dónde lo encuentro?**  
En entornos Windows con Active Directory donde SMB utiliza NTLM y existen configuraciones que permiten autenticación relayable.

**¿Por qué me afecta?**  
Puede permitir que un atacante reutilice una autenticación legítima para acceder a otros sistemas con los privilegios de la cuenta comprometida.

**¿Cómo se soluciona?**  
Reducir o deshabilitar NTLM cuando sea posible, habilitar protecciones contra relay como SMB signing, aplicar segmentación de red y monitorear autenticaciones anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría interceptar una autenticación NTLM y reenviarla a un servicio SMB susceptible para obtener acceso utilizando la identidad de la víctima.


## NTLM Relay

**¿Qué es?**  
Técnica que reenvía una autenticación NTLM válida desde un sistema o usuario hacia otro servicio que acepta NTLM, permitiendo abusar de la autenticación sin necesidad de obtener la contraseña.

**¿Dónde lo encuentro?**  
En redes Windows y Active Directory donde NTLM continúa habilitado y los servicios carecen de protecciones suficientes contra ataques de relay.

**¿Por qué me afecta?**  
Puede convertir una autenticación legítima en acceso no autorizado a otros servicios y facilitar movimiento lateral o acciones con privilegios elevados.

**¿Cómo se soluciona?**  
Reducir NTLM, habilitar mecanismos de protección contra relay, utilizar SMB signing y reforzar la autenticación y segmentación de red.

**¿Cómo lo usaría un atacante en mi contra?**  
Capturaría o induciría una autenticación NTLM y trataría de reenviarla a un servicio vulnerable para actuar utilizando los permisos asociados a esa identidad.


## Pass-the-Hash

**¿Qué es?**  
Técnica que permite autenticarse en determinados servicios utilizando un hash de contraseña obtenido de una cuenta, sin necesidad de conocer la contraseña original.

**¿Dónde lo encuentro?**  
Principalmente en entornos Windows donde se utilizan mecanismos de autenticación compatibles con hashes NTLM.

**¿Por qué me afecta?**  
El robo de un hash puede convertirse directamente en acceso a otros sistemas si la cuenta tiene permisos suficientes y el entorno no cuenta con controles adecuados.

**¿Cómo se soluciona?**  
Proteger las credenciales privilegiadas, limitar reutilización de cuentas administrativas, aplicar políticas de mínimo privilegio y utilizar mecanismos modernos de autenticación cuando estén disponibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras obtener el hash de una cuenta, intentaría utilizarlo para autenticarse en otros sistemas sin tener que descubrir la contraseña original.


## Pass-the-Ticket

**¿Qué es?**  
Técnica que consiste en reutilizar un ticket de Kerberos obtenido de una cuenta comprometida para autenticarse ante servicios del entorno sin conocer necesariamente su contraseña.

**¿Dónde lo encuentro?**  
En entornos Windows con Active Directory y Kerberos, especialmente cuando un atacante consigue acceso a tickets válidos en un sistema comprometido.

**¿Por qué me afecta?**  
Puede permitir acceso a recursos y servicios utilizando los privilegios asociados al ticket, dificultando distinguir la actividad maliciosa de una autenticación legítima.

**¿Cómo se soluciona?**  
Proteger sistemas y credenciales privilegiadas, limitar privilegios, controlar la duración y uso de tickets y monitorear autenticaciones Kerberos anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Obtendría un ticket válido de una cuenta comprometida y trataría de reutilizarlo para acceder a servicios autorizados para esa identidad.


## Kerberoasting

**¿Qué es?**  
Técnica que aprovecha cuentas de servicio de Active Directory asociadas a nombres principales de servicio (SPN) para obtener material de autenticación Kerberos que puede intentar recuperarse mediante ataques offline contra contraseñas débiles.

**¿Dónde lo encuentro?**  
En dominios Active Directory que contienen cuentas de servicio con SPN y contraseñas susceptibles de ser adivinadas o recuperadas mediante cracking offline.

**¿Por qué me afecta?**  
Una cuenta de servicio comprometida puede tener privilegios elevados y proporcionar una vía para escalar privilegios o moverse lateralmente dentro del dominio.

**¿Cómo se soluciona?**  
Usar contraseñas largas y resistentes para cuentas de servicio, aplicar mínimo privilegio, preferir cuentas administradas cuando sea posible y monitorear solicitudes Kerberos anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Identificaría cuentas de servicio asociadas a SPN, solicitaría tickets de servicio y utilizaría el material obtenido para intentar recuperar offline la contraseña de una cuenta vulnerable.


## AS-REP Roasting

**¿Qué es?**  
Técnica que aprovecha cuentas de Active Directory configuradas para no requerir preautenticación Kerberos, permitiendo obtener una respuesta AS-REP que puede someterse a ataques offline contra la contraseña.

**¿Dónde lo encuentro?**  
En dominios Active Directory donde existen cuentas con la opción de no requerir preautenticación Kerberos habilitada.

**¿Por qué me afecta?**  
Una contraseña débil puede ser recuperada offline y proporcionar acceso a una cuenta válida, que posteriormente podría utilizarse para movimiento lateral o escalada de privilegios.

**¿Cómo se soluciona?**  
Mantener habilitada la preautenticación Kerberos, utilizar contraseñas robustas, aplicar mínimo privilegio y revisar periódicamente las cuentas configuradas sin preautenticación.

**¿Cómo lo usaría un atacante en mi contra?**  
Identificaría cuentas sin preautenticación, obtendría respuestas Kerberos asociadas y trataría de recuperar offline las contraseñas mediante técnicas de cracking.
