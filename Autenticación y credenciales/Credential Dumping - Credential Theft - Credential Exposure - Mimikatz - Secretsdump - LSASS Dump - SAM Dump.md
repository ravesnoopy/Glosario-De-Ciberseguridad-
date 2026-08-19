
## Credential Dumping

**¿Qué es?**  
Técnica utilizada para extraer credenciales, hashes, tokens u otro material de autenticación almacenado o presente en memoria dentro de un sistema.

**¿Dónde lo encuentro?**  
En sistemas comprometidos, procesos de autenticación, archivos de credenciales, registros del sistema y herramientas utilizadas durante ataques o análisis forense.

**¿Por qué me afecta?**  
Las credenciales obtenidas pueden permitir acceso a otros sistemas, escalada de privilegios, movimiento lateral o suplantación de usuarios.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, proteger credenciales privilegiadas, habilitar controles de seguridad del sistema y monitorear accesos anómalos a procesos y almacenes de credenciales.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras comprometer un equipo, intentaría extraer credenciales para ampliar su acceso dentro del sistema o utilizarlas contra otros recursos.


## Credential Theft

**¿Qué es?**  
Robo de credenciales de autenticación, como contraseñas, tokens, claves o hashes, con el objetivo de utilizarlas para acceder a recursos protegidos.

**¿Dónde lo encuentro?**  
En campañas de phishing, malware, sistemas comprometidos, navegadores, aplicaciones, archivos y otros lugares donde puedan almacenarse o transmitirse credenciales.

**¿Por qué me afecta?**  
Una credencial robada puede permitir que un atacante se haga pasar por un usuario legítimo y evada controles que dependen únicamente de la autenticación.

**¿Cómo se soluciona?**  
Utilizar MFA, proteger los almacenes de credenciales, aplicar mínimo privilegio, evitar reutilización de contraseñas y monitorear autenticaciones sospechosas.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría obtener credenciales mediante phishing, malware, técnicas de extracción o acceso a sistemas comprometidos para utilizarlas posteriormente.


## Credential Exposure

**¿Qué es?**  
Exposición accidental o involuntaria de credenciales en ubicaciones donde personas o procesos no autorizados pueden acceder a ellas.

**¿Dónde lo encuentro?**  
En archivos de configuración, repositorios, scripts, registros, variables de entorno, documentos, bases de datos o sistemas de almacenamiento mal configurados.

**¿Por qué me afecta?**  
Las credenciales expuestas pueden proporcionar acceso directo a sistemas, aplicaciones, servicios o información sensible sin necesidad de explotar una vulnerabilidad adicional.

**¿Cómo se soluciona?**  
Evitar almacenar secretos en código o repositorios, utilizar gestores de secretos, restringir permisos y rotar inmediatamente las credenciales que hayan sido expuestas.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría credenciales expuestas en sistemas accesibles para obtener acceso legítimo a servicios y ampliar posteriormente su alcance.


## Mimikatz

**¿Qué es?**  
Herramienta de seguridad conocida por su capacidad para interactuar con mecanismos de autenticación de Windows y extraer o manipular determinados materiales de credenciales.

**¿Dónde lo encuentro?**  
En pruebas de penetración, laboratorios de seguridad, análisis de incidentes y también en ataques contra entornos Windows comprometidos.

**¿Por qué me afecta?**  
Su uso sobre un sistema comprometido puede permitir obtener material de autenticación y facilitar técnicas como Credential Dumping, Pass-the-Hash o Pass-the-Ticket.

**¿Cómo se soluciona?**  
Reducir privilegios administrativos, proteger procesos y credenciales, habilitar controles de seguridad de Windows y monitorear comportamientos asociados con extracción de credenciales.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de obtener los privilegios necesarios, podría utilizarla para intentar obtener material de autenticación y reutilizarlo para acceder a otros recursos.


## Secretsdump

**¿Qué es?**  
Herramienta de Impacket utilizada para extraer determinados secretos y material de autenticación de sistemas Windows, incluyendo información relacionada con SAM, SYSTEM y Active Directory.

**¿Dónde lo encuentro?**  
En laboratorios de seguridad, pruebas de penetración, investigación de incidentes y entornos comprometidos donde se utilizan técnicas de extracción de credenciales.

**¿Por qué me afecta?**  
La información obtenida puede permitir recuperar hashes de cuentas y facilitar ataques posteriores de autenticación o movimiento lateral.

**¿Cómo se soluciona?**  
Proteger cuentas privilegiadas, restringir acceso administrativo remoto, aplicar segmentación y monitorear actividades de extracción de credenciales y acceso a almacenes sensibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Con los permisos necesarios, intentaría extraer información de autenticación del sistema o dominio para obtener material reutilizable en fases posteriores del ataque.


## LSASS Dump

**¿Qué es?**  
Técnica que consiste en obtener una copia de la memoria del proceso `LSASS`, que administra funciones de autenticación en Windows y puede contener material sensible relacionado con sesiones activas.

**¿Dónde lo encuentro?**  
En sistemas Windows durante investigaciones forenses, pruebas de seguridad o ataques donde un adversario intenta obtener credenciales presentes en memoria.

**¿Por qué me afecta?**  
El acceso no autorizado a la memoria de LSASS puede exponer credenciales o tokens que permitan suplantar sesiones y acceder a otros recursos.

**¿Cómo se soluciona?**  
Proteger LSASS mediante mecanismos como Credential Guard cuando sea compatible, limitar privilegios administrativos y monitorear accesos anómalos al proceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría obtener un volcado de memoria de LSASS para buscar material de autenticación que pueda reutilizar posteriormente.


## SAM Dump

**¿Qué es?**  
Técnica de extracción de información del archivo `SAM` de Windows, que almacena datos relacionados con las cuentas locales y sus hashes de contraseñas.

**¿Dónde lo encuentro?**  
En sistemas Windows, donde la base de datos SAM se utiliza para gestionar información de autenticación de cuentas locales.

**¿Por qué me afecta?**  
La obtención de sus hashes puede facilitar ataques offline contra contraseñas o técnicas de autenticación que utilizan hashes.

**¿Cómo se soluciona?**  
Restringir privilegios administrativos, proteger el sistema operativo y sus archivos sensibles, utilizar contraseñas robustas y monitorear accesos sospechosos a la SAM.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras obtener privilegios suficientes, intentaría extraer los hashes de las cuentas locales para intentar recuperar sus contraseñas o reutilizar los hashes obtenidos.
