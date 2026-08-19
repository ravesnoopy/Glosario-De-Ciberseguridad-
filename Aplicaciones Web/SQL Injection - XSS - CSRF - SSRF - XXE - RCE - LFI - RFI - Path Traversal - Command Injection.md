
## SQL Injection

**¿Qué es?**  
Vulnerabilidad que ocurre cuando una aplicación incorpora datos controlados por el usuario en consultas SQL sin una validación o parametrización adecuada, permitiendo alterar la consulta original.

**¿Dónde lo encuentro?**  
En aplicaciones web y servicios que interactúan con bases de datos mediante entradas como formularios, parámetros URL, búsquedas o APIs.

**¿Por qué me afecta?**  
Puede permitir acceder, modificar o eliminar información de la base de datos y, dependiendo del entorno, comprometer otros componentes de la aplicación.

**¿Cómo se soluciona?**  
Utilizar consultas parametrizadas o prepared statements, validar las entradas, aplicar el principio de mínimo privilegio a las cuentas de base de datos y mantener componentes actualizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Manipularía entradas controladas por el usuario para modificar consultas SQL y obtener acceso no autorizado a datos o ejecutar operaciones que la aplicación no debería permitir.


## XSS

**¿Qué es?**  
Cross-Site Scripting es una vulnerabilidad que permite inyectar contenido ejecutable, normalmente JavaScript, en páginas web que posteriormente son procesadas por el navegador de otros usuarios.

**¿Dónde lo encuentro?**  
En aplicaciones web que muestran contenido proporcionado por usuarios sin aplicar correctamente validación, codificación de salida o controles de seguridad.

**¿Por qué me afecta?**  
Puede permitir robar sesiones, manipular contenido visible, realizar acciones en nombre de una víctima o capturar información accesible desde su navegador.

**¿Cómo se soluciona?**  
Aplicar codificación contextual de salida, validar entradas cuando corresponda, utilizar políticas como Content Security Policy y configurar correctamente las cookies de sesión.

**¿Cómo lo usaría un atacante en mi contra?**  
Inyectaría contenido malicioso en una aplicación vulnerable para conseguir que el navegador de otra persona lo ejecute bajo el contexto de confianza del sitio.


## CSRF

**¿Qué es?**  
Cross-Site Request Forgery es un ataque que induce a un usuario autenticado a realizar una acción no deseada en una aplicación donde mantiene una sesión válida.

**¿Dónde lo encuentro?**  
En aplicaciones web que aceptan solicitudes que modifican información o ejecutan acciones importantes sin verificar adecuadamente que la solicitud provenga de una interacción legítima del usuario.

**¿Por qué me afecta?**  
Puede provocar cambios de configuración, modificaciones de datos o acciones realizadas con los privilegios de una víctima autenticada.

**¿Cómo se soluciona?**  
Utilizar tokens anti-CSRF, configurar adecuadamente las cookies mediante `SameSite` y verificar el origen de solicitudes cuando sea apropiado.

**¿Cómo lo usaría un atacante en mi contra?**  
Prepararía una solicitud maliciosa que, al ser procesada por un usuario autenticado, podría ejecutar una acción en la aplicación utilizando automáticamente su sesión.


## SSRF

**¿Qué es?**  
Server-Side Request Forgery es una vulnerabilidad que permite inducir a un servidor a realizar solicitudes hacia recursos elegidos o influenciados por un atacante.

**¿Dónde lo encuentro?**  
En funciones que permiten al servidor obtener URLs o recursos externos, como importadores, webhooks, validadores de URLs, generadores de imágenes o integraciones con APIs.

**¿Por qué me afecta?**  
Puede utilizarse para acceder a servicios internos que no deberían estar expuestos directamente a Internet y, en ciertos entornos, obtener información sensible o ampliar el alcance del ataque.

**¿Cómo se soluciona?**  
Aplicar listas permitidas de destinos, validar estrictamente URLs y direcciones, bloquear accesos a redes internas y metadatos de infraestructura cuando no sean necesarios y controlar las solicitudes salientes.

**¿Cómo lo usaría un atacante en mi contra?**  
Manipularía una función que realiza solicitudes desde el servidor para intentar alcanzar servicios internos o recursos que normalmente no son accesibles desde el exterior.


## XXE

**¿Qué es?**  
XML External Entity es una vulnerabilidad que ocurre cuando un procesador XML permite entidades externas controladas o influenciadas por datos no confiables.

**¿Dónde lo encuentro?**  
En aplicaciones, APIs y servicios que procesan documentos XML mediante configuraciones que permiten entidades externas o funcionalidades XML innecesarias.

**¿Por qué me afecta?**  
Puede permitir la lectura de archivos locales, realizar solicitudes desde el servidor y, dependiendo de la configuración, facilitar ataques contra otros sistemas.

**¿Cómo se soluciona?**  
Deshabilitar entidades externas y funcionalidades XML innecesarias, utilizar analizadores XML configurados de forma segura y mantener actualizadas las bibliotecas utilizadas para procesar XML.

**¿Cómo lo usaría un atacante en mi contra?**  
Enviaría un documento XML especialmente construido para provocar que el servidor procese una entidad externa y acceda a un recurso que debería permanecer protegido.


## RCE

**¿Qué es?**  
Remote Code Execution es una vulnerabilidad o capacidad de ataque que permite ejecutar código arbitrario en un sistema remoto con los privilegios del componente comprometido.

**¿Dónde lo encuentro?**  
En aplicaciones, servidores, servicios, frameworks o componentes vulnerables que procesan entradas no confiables de manera insegura.

**¿Por qué me afecta?**  
Puede proporcionar un nivel de acceso crítico, permitiendo al atacante controlar procesos, acceder a información, instalar herramientas maliciosas o avanzar hacia otros sistemas.

**¿Cómo se soluciona?**  
Corregir vulnerabilidades conocidas, actualizar componentes, validar entradas, reducir privilegios y aislar servicios para limitar el impacto de una posible ejecución de código.

**¿Cómo lo usaría un atacante en mi contra?**  
Aprovecharía una vulnerabilidad para conseguir que un servicio remoto ejecute instrucciones bajo los privilegios de la aplicación o sistema comprometido.


## LFI

**¿Qué es?**  
Local File Inclusion es una vulnerabilidad que permite a un atacante influir en qué archivos locales intenta cargar una aplicación, debido a una gestión insegura de rutas o recursos.

**¿Dónde lo encuentro?**  
Principalmente en aplicaciones web que reciben mediante parámetros el nombre o la ruta de archivos que deben incluir, cargar o mostrar.

**¿Por qué me afecta?**  
Puede permitir acceder a archivos sensibles del servidor y, en determinadas condiciones, contribuir a comprometer la ejecución de la aplicación.

**¿Cómo se soluciona?**  
Evitar que el usuario controle directamente las rutas, utilizar listas permitidas de archivos, normalizar rutas y aplicar permisos mínimos al proceso de la aplicación.

**¿Cómo lo usaría un atacante en mi contra?**  
Manipularía un parámetro utilizado para cargar archivos con el objetivo de acceder a información local que la aplicación no debería exponer.


## RFI

**¿Qué es?**  
Remote File Inclusion es una vulnerabilidad que permite a una aplicación incluir o cargar un recurso remoto controlado por un atacante cuando su mecanismo de inclusión acepta fuentes externas.

**¿Dónde lo encuentro?**  
En aplicaciones que permiten seleccionar dinámicamente archivos o recursos y utilizan mecanismos capaces de cargar contenido desde ubicaciones remotas.

**¿Por qué me afecta?**  
Puede permitir que contenido controlado por un atacante sea incorporado a la aplicación y, en entornos vulnerables, llegar a producir ejecución de código.

**¿Cómo se soluciona?**  
Deshabilitar la inclusión remota cuando no sea necesaria, utilizar listas permitidas de recursos y validar estrictamente los archivos y ubicaciones que puede utilizar la aplicación.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría conseguir que la aplicación cargara un recurso remoto bajo su control para introducir contenido malicioso en el procesamiento del servidor.


## Path Traversal

**¿Qué es?**  
Path Traversal es una vulnerabilidad que permite manipular rutas de archivos para escapar del directorio previsto por la aplicación y acceder a ubicaciones fuera del alcance autorizado.

**¿Dónde lo encuentro?**  
En aplicaciones que construyen rutas de archivos a partir de entradas proporcionadas por usuarios, como descargas, visualización de documentos o carga de recursos.

**¿Por qué me afecta?**  
Puede exponer archivos de configuración, credenciales, código fuente u otra información sensible almacenada en el sistema.

**¿Cómo se soluciona?**  
Normalizar y validar rutas, utilizar listas permitidas, restringir el directorio accesible y evitar construir rutas directamente a partir de entradas no confiables.

**¿Cómo lo usaría un atacante en mi contra?**  
Manipularía parámetros relacionados con archivos o directorios para intentar salir de la ubicación permitida y acceder a recursos protegidos del sistema.


## Command Injection

**¿Qué es?**  
Command Injection es una vulnerabilidad que ocurre cuando una aplicación incorpora datos controlados por el usuario en comandos del sistema operativo sin separar correctamente los datos de las instrucciones.

**¿Dónde lo encuentro?**  
En aplicaciones que ejecutan comandos del sistema para realizar tareas como procesamiento de archivos, administración de servicios o ejecución de herramientas externas.

**¿Por qué me afecta?**  
Puede permitir ejecutar comandos con los privilegios del proceso afectado y comprometer la confidencialidad, integridad y disponibilidad del sistema.

**¿Cómo se soluciona?**  
Evitar ejecutar comandos del sistema cuando exista una alternativa segura, utilizar APIs específicas, separar argumentos de datos, validar entradas y aplicar mínimo privilegio.

**¿Cómo lo usaría un atacante en mi contra?**  
Manipularía una entrada procesada por la aplicación para conseguir que el sistema interprete parte de sus datos como instrucciones adicionales.
