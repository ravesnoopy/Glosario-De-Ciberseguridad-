!banner 

# PHP / ASP / ASP.NET / ASPX / JavaScript / HTML / CSS

### PHP

**¿Qué es?**  
Lenguaje de programación utilizado principalmente para desarrollar aplicaciones web del lado del servidor.

**¿Dónde lo encuentro?**  
En servidores y aplicaciones web, normalmente en archivos `.php`.

**¿Por qué me afecta?**  
Una aplicación PHP vulnerable puede permitir ataques como inyección SQL, ejecución de código o acceso no autorizado.

**¿Cómo se soluciona?**  
Mantener PHP y sus dependencias actualizados, validar entradas, utilizar consultas parametrizadas y aplicar una configuración segura.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar vulnerabilidades de una aplicación PHP para manipular solicitudes, acceder a información o ejecutar acciones no autorizadas.

---

### ASP

**¿Qué es?**  
Tecnología de Microsoft utilizada para generar páginas web dinámicas desde el servidor. Es anterior a ASP.NET y actualmente se considera una tecnología heredada.

**¿Dónde lo encuentro?**  
Principalmente en aplicaciones web antiguas alojadas en IIS, normalmente mediante archivos `.asp`.

**¿Por qué me afecta?**  
Las aplicaciones ASP heredadas pueden utilizar componentes obsoletos o configuraciones inseguras que aumentan la superficie de ataque.

**¿Cómo se soluciona?**  
Mantener el servidor actualizado, reducir la exposición y, cuando sea posible, migrar aplicaciones heredadas a tecnologías modernas y soportadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar vulnerabilidades en aplicaciones ASP expuestas para obtener información o conseguir acceso no autorizado.

---

### ASP.NET

**¿Qué es?**  
Framework de Microsoft para desarrollar aplicaciones web que procesan solicitudes y generan contenido desde el servidor.

**¿Dónde lo encuentro?**  
En aplicaciones web alojadas en servidores como IIS y desarrolladas dentro del ecosistema .NET.

**¿Por qué me afecta?**  
Una aplicación ASP.NET mal desarrollada o configurada puede presentar vulnerabilidades relacionadas con autenticación, autorización, sesiones o entradas de usuario.

**¿Cómo se soluciona?**  
Mantener .NET y sus dependencias actualizados, implementar controles adecuados de autenticación y autorización y validar correctamente las entradas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar vulnerabilidades de la aplicación para acceder a funciones restringidas, manipular datos o comprometer otros componentes.

---

### ASPX

**¿Qué es?**  
Extensión utilizada habitualmente por páginas web desarrolladas con ASP.NET. No es un lenguaje de programación independiente.

**¿Dónde lo encuentro?**  
En aplicaciones ASP.NET alojadas en servidores web, especialmente IIS. Por ejemplo, `login.aspx` o `admin.aspx`.

**¿Por qué me afecta?**  
Una página ASPX puede formar parte de una aplicación vulnerable o exponer funciones que no deberían estar disponibles para usuarios no autorizados.

**¿Cómo se soluciona?**  
Aplicar correctamente autenticación y autorización, mantener la aplicación actualizada y evitar exponer funciones administrativas innecesariamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar páginas ASPX accesibles y analizarlas en busca de controles de acceso deficientes o vulnerabilidades.

---

### JavaScript

**¿Qué es?**  
Lenguaje de programación utilizado para añadir comportamiento e interacción a páginas y aplicaciones web.

**¿Dónde lo encuentro?**  
En páginas web, archivos `.js` y aplicaciones que ejecutan código JavaScript.

**¿Por qué me afecta?**  
Una implementación insegura puede contribuir a vulnerabilidades como XSS, manipulación del DOM o exposición de información.

**¿Cómo se soluciona?**  
Validar y escapar correctamente los datos, evitar insertar contenido no confiable en el DOM, mantener las dependencias actualizadas y utilizar controles como CSP cuando corresponda.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede introducir JavaScript malicioso para ejecutarlo en el navegador de otra persona, robar información accesible desde su sesión o realizar acciones en su nombre.

---

### HTML

**¿Qué es?**  
Lenguaje de marcado utilizado para estructurar el contenido de las páginas web.

**¿Dónde lo encuentro?**  
En prácticamente cualquier página o aplicación web, donde es procesado por el navegador.

**¿Por qué me afecta?**  
El contenido HTML puede formar parte de la superficie de ataque, especialmente cuando incorpora datos proporcionados por usuarios sin procesarlos correctamente.

**¿Cómo se soluciona?**  
Escapar o sanitizar correctamente el contenido no confiable y aplicar controles de seguridad cuando la aplicación genere HTML dinámicamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar insertar contenido manipulado en páginas vulnerables para alterar su comportamiento o facilitar ataques como XSS.

---

### CSS

**¿Qué es?**  
Lenguaje utilizado para definir la apariencia y presentación visual de las páginas web.

**¿Dónde lo encuentro?**  
En archivos `.css`, documentos HTML y aplicaciones web.

**¿Por qué me afecta?**  
CSS normalmente no permite comprometer un sistema por sí solo, pero puede contribuir a engaños visuales o combinarse con otras vulnerabilidades.

**¿Cómo se soluciona?**  
Evitar depender de contenido no confiable para generar estilos y aplicar controles de seguridad adecuados en la aplicación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular la apariencia de una página para engañar a usuarios o combinar técnicas de presentación con otras vulnerabilidades web.
