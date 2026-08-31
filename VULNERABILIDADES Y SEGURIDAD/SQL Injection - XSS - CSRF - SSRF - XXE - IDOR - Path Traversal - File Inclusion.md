# SQL Injection

**¿Qué es?**  
SQL Injection es una vulnerabilidad que ocurre cuando una aplicación incorpora datos controlados por el usuario en consultas SQL sin aplicar controles adecuados, permitiendo alterar la consulta prevista.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs y servicios que interactúan con bases de datos mediante consultas construidas de forma insegura.

**¿Por qué me afecta?**  
Puede permitir acceder, modificar o eliminar información de una base de datos y, dependiendo del entorno, afectar otros componentes de la aplicación.

**¿Cómo se soluciona?**  
Utilizando consultas parametrizadas, prepared statements, validación de entradas y cuentas de base de datos con privilegios mínimos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular entradas que llegan a consultas SQL para intentar modificar su comportamiento y acceder a datos que no debería poder consultar.

---

# XSS

**¿Qué es?**  
XSS (Cross-Site Scripting) es una vulnerabilidad que permite que contenido controlado por un atacante sea interpretado como código ejecutable por el navegador de otro usuario.

**¿Dónde lo encuentro?**  
En aplicaciones web que muestran contenido proporcionado por usuarios sin aplicar correctamente validación, sanitización o codificación de salida.

**¿Por qué me afecta?**  
Puede permitir ejecutar acciones en el contexto del navegador de una víctima, modificar contenido de una página o afectar sesiones y cuentas.

**¿Cómo se soluciona?**  
Aplicando output encoding según el contexto, sanitización cuando sea necesaria, Content Security Policy y validación adecuada de entradas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar introducir contenido malicioso en una aplicación para que sea interpretado por el navegador de otros usuarios.

---

# CSRF

**¿Qué es?**  
CSRF (Cross-Site Request Forgery) es una vulnerabilidad que permite inducir a un usuario autenticado a realizar una acción en una aplicación sin haberla solicitado intencionalmente.

**¿Dónde lo encuentro?**  
En aplicaciones web que utilizan sesiones basadas en cookies y no verifican adecuadamente el origen o intención de determinadas solicitudes.

**¿Por qué me afecta?**  
Una víctima autenticada podría ejecutar acciones no deseadas utilizando sus propios permisos.

**¿Cómo se soluciona?**  
Utilizando tokens anti-CSRF, configurando correctamente las cookies `SameSite` y verificando mecanismos como `Origin` o `Referer` cuando corresponda.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede inducir a una víctima autenticada a visitar contenido que provoque solicitudes hacia una aplicación donde mantiene una sesión activa.

---

# SSRF

**¿Qué es?**  
SSRF (Server-Side Request Forgery) es una vulnerabilidad que permite influir en las solicitudes que un servidor realiza hacia otros recursos o sistemas.

**¿Dónde lo encuentro?**  
En aplicaciones y APIs que reciben URLs o destinos controlados por usuarios y posteriormente realizan solicitudes desde el servidor.

**¿Por qué me afecta?**  
Puede permitir acceder a recursos internos que no deberían estar disponibles directamente desde Internet o interactuar con servicios internos.

**¿Cómo se soluciona?**  
Restringiendo destinos permitidos, validando URLs, controlando protocolos y evitando que el servidor pueda acceder innecesariamente a redes o servicios internos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar hacer que un servidor realice solicitudes hacia recursos internos o destinos que normalmente no serían accesibles desde el exterior.

---

# XXE

**¿Qué es?**  
XXE (XML External Entity) es una vulnerabilidad que ocurre cuando un procesador XML permite utilizar entidades externas provenientes de datos XML no confiables.

**¿Dónde lo encuentro?**  
En aplicaciones y APIs que procesan XML mediante parsers configurados de forma insegura.

**¿Por qué me afecta?**  
Puede provocar exposición de información, solicitudes hacia recursos internos o comportamientos inesperados durante el procesamiento del XML.

**¿Cómo se soluciona?**  
Deshabilitando entidades externas y DTD cuando no sean necesarias y utilizando configuraciones seguras para los parsers XML.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede proporcionar XML especialmente construido para intentar provocar que el parser procese referencias externas no autorizadas.

---

# IDOR

**¿Qué es?**  
IDOR (Insecure Direct Object Reference) es una vulnerabilidad que ocurre cuando una aplicación permite acceder directamente a objetos o recursos mediante identificadores sin verificar correctamente la autorización.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs y sistemas que utilizan identificadores para acceder a registros, archivos, cuentas u otros recursos.

**¿Por qué me afecta?**  
Puede permitir que un usuario acceda a información perteneciente a otro usuario simplemente modificando un identificador.

**¿Cómo se soluciona?**  
Implementando comprobaciones de autorización del lado del servidor para cada recurso solicitado y aplicando mínimo privilegio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar identificadores de recursos en una solicitud para intentar acceder a objetos que pertenecen a otros usuarios.

---

# Path Traversal

**¿Qué es?**  
Path Traversal es una vulnerabilidad que permite manipular una ruta proporcionada a una aplicación para intentar acceder a archivos o directorios fuera de la ubicación prevista.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, servidores de archivos y sistemas que construyen rutas utilizando entradas controladas por usuarios.

**¿Por qué me afecta?**  
Puede permitir el acceso no autorizado a archivos o información almacenada fuera del directorio que la aplicación debería poder utilizar.

**¿Cómo se soluciona?**  
Validando las rutas, utilizando listas permitidas, normalizando correctamente los paths y restringiendo los permisos del proceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular parámetros relacionados con archivos o directorios para intentar escapar de la ubicación permitida por la aplicación.

---

# File Inclusion

**¿Qué es?**  
File Inclusion es una vulnerabilidad que ocurre cuando una aplicación permite que una entrada controlada por el usuario determine qué archivo debe incluir o cargar sin aplicar controles adecuados.

**¿Dónde lo encuentro?**  
En aplicaciones web que cargan archivos, plantillas, módulos o recursos dinámicamente a partir de parámetros externos.

**¿Por qué me afecta?**  
Puede permitir acceder a archivos no autorizados o, dependiendo de la implementación, provocar la ejecución de contenido controlado por un atacante.

**¿Cómo se soluciona?**  
Utilizando listas permitidas de archivos, evitando incluir rutas controladas directamente por usuarios y restringiendo los permisos del proceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular parámetros utilizados para seleccionar archivos e intentar cargar recursos que la aplicación no debería permitir.
