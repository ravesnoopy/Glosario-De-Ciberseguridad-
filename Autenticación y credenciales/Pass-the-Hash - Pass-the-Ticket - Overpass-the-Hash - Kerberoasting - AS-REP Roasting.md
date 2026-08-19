
## Pass-the-Hash

**¿Qué es?**  
Técnica que permite autenticarse en determinados servicios utilizando el hash de una contraseña obtenida de una cuenta, sin necesidad de conocer la contraseña original.

**¿Dónde lo encuentro?**  
Principalmente en entornos Windows que utilizan mecanismos de autenticación compatibles con NTLM.

**¿Por qué me afecta?**  
El robo de un hash puede convertirse en acceso no autorizado si la cuenta tiene permisos sobre otros sistemas o recursos.

**¿Cómo se soluciona?**  
Proteger las credenciales privilegiadas, limitar el uso de cuentas administrativas, aplicar mínimo privilegio y utilizar mecanismos de autenticación más resistentes cuando sea posible.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras obtener un hash válido, intentaría utilizarlo para autenticarse en otros sistemas sin necesidad de recuperar la contraseña original.


## Pass-the-Ticket

**¿Qué es?**  
Técnica que consiste en reutilizar un ticket Kerberos válido obtenido de una cuenta comprometida para autenticarse ante servicios autorizados para esa identidad.

**¿Dónde lo encuentro?**  
En entornos Windows con Active Directory y Kerberos, especialmente en sistemas donde existen sesiones autenticadas y tickets almacenados.

**¿Por qué me afecta?**  
Un ticket comprometido puede permitir suplantar temporalmente una identidad y facilitar el acceso a recursos o movimiento lateral.

**¿Cómo se soluciona?**  
Proteger sistemas y cuentas privilegiadas, limitar privilegios, controlar la duración de tickets y monitorear autenticaciones Kerberos anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Obtendría un ticket de una sesión comprometida e intentaría reutilizarlo para acceder a los servicios disponibles para esa identidad.


## Overpass-the-Hash

**¿Qué es?**  
Técnica que utiliza material de autenticación derivado de una contraseña, como un hash NTLM, para obtener un ticket Kerberos y posteriormente autenticarse mediante Kerberos.

**¿Dónde lo encuentro?**  
En entornos Windows con Active Directory donde Kerberos es utilizado junto con mecanismos de autenticación compatibles con hashes NTLM.

**¿Por qué me afecta?**  
Permite transformar el compromiso de un hash en credenciales Kerberos utilizables, facilitando el acceso a servicios que dependen de Kerberos.

**¿Cómo se soluciona?**  
Proteger hashes y credenciales, reducir privilegios administrativos, limitar exposición de cuentas privilegiadas y monitorear comportamientos anómalos de autenticación Kerberos y NTLM.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de obtener el material de autenticación de una cuenta, intentaría utilizarlo para obtener un ticket Kerberos y acceder a servicios con la identidad comprometida.


## Kerberoasting

**¿Qué es?**  
Técnica que aprovecha cuentas de servicio de Active Directory asociadas a SPN para obtener tickets de servicio cuyo material puede someterse a ataques offline contra contraseñas débiles.

**¿Dónde lo encuentro?**  
En dominios Active Directory que contienen cuentas de servicio con SPN y credenciales susceptibles de ser recuperadas mediante ataques de contraseña.

**¿Por qué me afecta?**  
Una cuenta de servicio comprometida puede disponer de permisos elevados y proporcionar una vía para escalada de privilegios o movimiento lateral.

**¿Cómo se soluciona?**  
Utilizar contraseñas largas y resistentes, aplicar mínimo privilegio, emplear cuentas administradas cuando sea posible y revisar periódicamente las cuentas asociadas a SPN.

**¿Cómo lo usaría un atacante en mi contra?**  
Identificaría cuentas de servicio con SPN, solicitaría sus tickets y utilizaría el material obtenido para intentar recuperar offline las contraseñas de cuentas vulnerables.


## AS-REP Roasting

**¿Qué es?**  
Técnica que aprovecha cuentas de Active Directory configuradas sin preautenticación Kerberos para obtener respuestas AS-REP que pueden ser atacadas offline contra contraseñas débiles.

**¿Dónde lo encuentro?**  
En dominios Active Directory donde existen cuentas configuradas para no requerir preautenticación Kerberos.

**¿Por qué me afecta?**  
La recuperación de una contraseña puede proporcionar acceso a una cuenta válida y facilitar posteriormente el movimiento lateral o la escalada de privilegios.

**¿Cómo se soluciona?**  
Mantener habilitada la preautenticación Kerberos, utilizar contraseñas robustas, aplicar mínimo privilegio y revisar periódicamente las cuentas configuradas sin preautenticación.

**¿Cómo lo usaría un atacante en mi contra?**  
Identificaría cuentas sin preautenticación, obtendría sus respuestas Kerberos y trataría de recuperar offline las contraseñas asociadas.
