# Token

**¿Qué es?**  
Token es una estructura de seguridad de Windows que contiene información sobre la identidad, grupos, privilegios y permisos asociados con un proceso o sesión.

**¿Dónde lo encuentro?**  
En procesos, sesiones de usuario y mecanismos de autenticación de Windows.

**¿Por qué me afecta?**  
El token determina, en gran medida, qué recursos puede utilizar un proceso y qué acciones puede realizar en nombre de una identidad.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, protegiendo las cuentas privilegiadas y monitoreando comportamientos relacionados con tokens y privilegios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener, reutilizar o manipular tokens con mayores privilegios para ejecutar acciones bajo el contexto de otra identidad.

---

# Integrity Level

**¿Qué es?**  
Integrity Level es un mecanismo de seguridad de Windows que clasifica procesos y objetos según su nivel de confianza y restringe determinadas interacciones entre ellos.

**¿Dónde lo encuentro?**  
En procesos, archivos, objetos y sesiones de Windows, especialmente dentro de los mecanismos de User Account Control (UAC).

**¿Por qué me afecta?**  
Ayuda a impedir que procesos con un nivel de integridad inferior modifiquen determinados recursos protegidos.

**¿Cómo se soluciona?**  
Manteniendo configuraciones adecuadas de UAC, evitando ejecutar aplicaciones innecesariamente con privilegios elevados y aplicando mínimo privilegio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar elevar el Integrity Level de un proceso para obtener acceso a recursos que requieren mayores privilegios.

---

# User Session

**¿Qué es?**  
User Session es el contexto de ejecución asociado con un usuario mientras utiliza un sistema, incluyendo sus procesos, aplicaciones y recursos disponibles.

**¿Dónde lo encuentro?**  
En sistemas operativos, servidores, escritorios remotos y entornos donde existen múltiples usuarios conectados.

**¿Por qué me afecta?**  
Una sesión comprometida puede proporcionar a un atacante acceso a los recursos disponibles para el usuario que la inició.

**¿Cómo se soluciona?**  
Protegiendo las cuentas, controlando sesiones activas, aplicando políticas de bloqueo y cierre de sesión y monitoreando accesos sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una sesión existente o utilizar una sesión de un usuario legítimo para realizar acciones con sus permisos.

---

# Logon Session

**¿Qué es?**  
Logon Session es el contexto de seguridad creado por Windows cuando una identidad se autentica en el sistema.

**¿Dónde lo encuentro?**  
En sistemas Windows, eventos de seguridad, procesos, tokens y mecanismos de autenticación.

**¿Por qué me afecta?**  
Permite relacionar autenticaciones con usuarios, procesos y actividades realizadas durante una sesión.

**¿Cómo se soluciona?**  
Monitoreando eventos de inicio de sesión, aplicando controles de autenticación y protegiendo las credenciales y sesiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener o reutilizar información asociada con una sesión de autenticación para acceder a recursos sin volver a autenticarse de la manera esperada.

---

# Environment Variable

**¿Qué es?**  
Environment Variable es un valor almacenado por el sistema operativo o el entorno de ejecución que proporciona información de configuración a procesos y aplicaciones.

**¿Dónde lo encuentro?**  
En sistemas operativos, procesos, scripts, aplicaciones y configuraciones de usuario o sistema.

**¿Por qué me afecta?**  
Algunas variables pueden contener rutas, configuraciones o información sensible que influye en el comportamiento de aplicaciones y procesos.

**¿Cómo se soluciona?**  
Evitando almacenar secretos directamente en variables cuando existan alternativas más seguras, controlando quién puede modificarlas y revisando su contenido.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede consultar variables disponibles para obtener información sobre el entorno o intentar modificar aquellas que influyen en la ejecución de programas.

---

# PATH

**¿Qué es?**  
PATH es una Environment Variable que contiene una lista de directorios donde el sistema busca determinados ejecutables cuando se especifica un programa sin proporcionar su ruta completa.

**¿Dónde lo encuentro?**  
En sistemas operativos, especialmente Windows, y dentro de los entornos de ejecución de procesos.

**¿Por qué me afecta?**  
Una configuración insegura del PATH puede hacer que un programa ejecute un archivo incorrecto o no confiable cuando busca un ejecutable.

**¿Cómo se soluciona?**  
Utilizando rutas confiables, evitando directorios controlables por usuarios no privilegiados y revisando periódicamente la configuración del PATH.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar colocar un ejecutable con un nombre esperado en una ubicación prioritaria del PATH para conseguir que un proceso ejecute su archivo en lugar del legítimo.
