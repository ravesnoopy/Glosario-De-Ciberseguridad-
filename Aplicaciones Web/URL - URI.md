
## URL

**¿Qué es?**  
Uniform Resource Locator es una dirección que identifica la ubicación y el mecanismo de acceso a un recurso en una red, como una página web, archivo o servicio.

**¿Dónde lo encuentro?**  
En navegadores, aplicaciones web, APIs, configuraciones, correos electrónicos, registros de red y solicitudes HTTP.

**¿Por qué me afecta?**  
Las URLs forman parte de la superficie de ataque y pueden contener parámetros, rutas o destinos manipulables que intervienen en vulnerabilidades como phishing, SSRF, Open Redirect o Path Traversal.

**¿Cómo se soluciona?**  
Validar y restringir URLs cuando provengan de usuarios, utilizar listas permitidas de dominios cuando sea necesario y evitar confiar en sus componentes sin verificarlos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría manipular una URL para redirigir a una víctima, alterar parámetros, acceder a recursos no autorizados o hacer que una aplicación solicite un destino controlado por él.


## URI

**¿Qué es?**  
Uniform Resource Identifier es un identificador que permite distinguir un recurso mediante una secuencia estructurada de caracteres; una URL es un tipo de URI que además proporciona información para localizar o acceder al recurso.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, sistemas de identificación de recursos, enlaces, configuraciones y protocolos que utilizan identificadores estructurados.

**¿Por qué me afecta?**  
Una interpretación o validación incorrecta de URIs puede provocar problemas de control de acceso, redirecciones, filtrado de entradas o acceso a recursos no previstos.

**¿Cómo se soluciona?**  
Validar correctamente la estructura y los componentes del URI, normalizar cuando corresponda y aplicar controles de acceso independientemente de cómo se represente el recurso.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría manipular la estructura o representación de un URI para evadir validaciones, acceder a recursos no autorizados o alterar el comportamiento de una aplicación que lo procese incorrectamente.
