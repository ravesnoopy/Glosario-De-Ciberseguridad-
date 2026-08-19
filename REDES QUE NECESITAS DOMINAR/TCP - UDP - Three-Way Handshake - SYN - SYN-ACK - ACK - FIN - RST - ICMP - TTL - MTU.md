
## TCP

**¿Qué es?**  
Protocolo de transporte orientado a conexión que proporciona entrega confiable y ordenada de datos entre dos extremos.

**¿Dónde lo encuentro?**  
En aplicaciones web, correo electrónico, transferencia de archivos, administración remota y numerosos servicios de red.

**¿Por qué me afecta?**  
El análisis de TCP permite identificar conexiones, servicios, escaneos y comportamientos anómalos en la red.

**¿Cómo se soluciona?**  
Controlar los servicios TCP expuestos mediante firewalls, segmentación, autenticación y monitoreo de conexiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar conexiones TCP para explorar servicios, comunicarse con sistemas comprometidos o mantener sesiones con infraestructura externa.


## UDP

**¿Qué es?**  
Protocolo de transporte sin conexión que permite enviar datagramas sin establecer una sesión ni garantizar su entrega u orden.

**¿Dónde lo encuentro?**  
En DNS, DHCP, streaming, VoIP, servicios de descubrimiento y aplicaciones que priorizan rapidez sobre confiabilidad.

**¿Por qué me afecta?**  
Los servicios UDP pueden quedar expuestos y son relevantes en reconocimiento, ataques de denegación de servicio y análisis de tráfico.

**¿Cómo se soluciona?**  
Restringir los puertos UDP innecesarios, aplicar controles de tráfico y monitorear patrones anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría explorar servicios UDP, abusar de servicios expuestos o generar grandes volúmenes de tráfico.


## Three-Way Handshake

**¿Qué es?**  
Proceso utilizado por TCP para establecer una conexión mediante el intercambio de `SYN`, `SYN-ACK` y `ACK`.

**¿Dónde lo encuentro?**  
En conexiones TCP entre clientes y servidores y en capturas de tráfico de herramientas como Wireshark.

**¿Por qué me afecta?**  
Su análisis permite identificar intentos de conexión, conexiones incompletas y patrones asociados con reconocimiento o ataques.

**¿Cómo se soluciona?**  
Monitorear conexiones TCP y utilizar controles como firewalls e IDS/IPS para detectar comportamientos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar numerosos intentos de conexión para realizar reconocimiento o provocar agotamiento de recursos mediante determinados ataques.


## SYN

**¿Qué es?**  
Flag de TCP utilizada para iniciar una conexión y sincronizar los números de secuencia entre los dos extremos.

**¿Dónde lo encuentro?**  
En el inicio de conexiones TCP y en capturas de tráfico de red.

**¿Por qué me afecta?**  
Un volumen o patrón anómalo de paquetes `SYN` puede indicar reconocimiento o intentos de saturar recursos.

**¿Cómo se soluciona?**  
Monitorear tasas de `SYN`, aplicar controles de firewall y utilizar mecanismos de protección contra ataques de agotamiento de conexiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría enviar múltiples `SYN` para descubrir servicios o intentar consumir recursos de un servidor.


## SYN-ACK

**¿Qué es?**  
Flag de TCP que combina `SYN` y `ACK` y representa la respuesta del servidor a un `SYN` durante el establecimiento de una conexión.

**¿Dónde lo encuentro?**  
En el segundo paso del Three-Way Handshake de una conexión TCP.

**¿Por qué me afecta?**  
Su presencia permite analizar qué conexiones están siendo aceptadas y detectar patrones anómalos durante el establecimiento de sesiones.

**¿Cómo se soluciona?**  
Monitorear los patrones de handshake y aplicar controles de red contra conexiones sospechosas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría analizar respuestas `SYN-ACK` para identificar servicios accesibles y confirmar que determinados puertos responden.


## ACK

**¿Qué es?**  
Flag de TCP utilizada para indicar que un segmento recibido ha sido reconocido correctamente.

**¿Dónde lo encuentro?**  
Durante el establecimiento y la comunicación de conexiones TCP.

**¿Por qué me afecta?**  
Los patrones de `ACK` ayudan a analizar el estado de conexiones y detectar tráfico TCP anómalo.

**¿Cómo se soluciona?**  
Monitorear las conexiones TCP y aplicar reglas de filtrado adecuadas según el comportamiento esperado.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar paquetes `ACK` con patrones específicos para reconocimiento, evasión de filtros o manipulación del tráfico.


## FIN

**¿Qué es?**  
Flag de TCP utilizada para indicar que un extremo desea finalizar de forma ordenada una conexión.

**¿Dónde lo encuentro?**  
En el cierre normal de conexiones TCP y en capturas de tráfico.

**¿Por qué me afecta?**  
Los patrones de `FIN` pueden ayudar a determinar cómo se establecen y terminan las conexiones y detectar comportamientos anómalos.

**¿Cómo se soluciona?**  
Analizar secuencias TCP y establecer controles para identificar tráfico de cierre inusual.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar paquetes `FIN` con patrones específicos durante técnicas de reconocimiento o para intentar evadir determinados filtros.


## RST

**¿Qué es?**  
Flag de TCP utilizada para reiniciar o rechazar una conexión de forma inmediata.

**¿Dónde lo encuentro?**  
En conexiones TCP rechazadas, interrumpidas o que intentan acceder a servicios que no aceptan la conexión.

**¿Por qué me afecta?**  
Un patrón elevado o inesperado de `RST` puede revelar escaneos, servicios inaccesibles o problemas de comunicación.

**¿Cómo se soluciona?**  
Analizar los patrones de `RST` junto con otros eventos de red y configurar correctamente los controles de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar paquetes `RST` para interrumpir conexiones o como parte de técnicas de reconocimiento y evasión.


## ICMP

**¿Qué es?**  
Protocolo utilizado principalmente para enviar mensajes de control, diagnóstico y errores relacionados con las comunicaciones IP.

**¿Dónde lo encuentro?**  
En herramientas como `ping` y `traceroute`, routers, firewalls y dispositivos de red.

**¿Por qué me afecta?**  
ICMP puede proporcionar información sobre sistemas y rutas de red y también puede ser utilizado de forma abusiva.

**¿Cómo se soluciona?**  
Filtrar tipos de ICMP según las necesidades del entorno y monitorear patrones anómalos sin bloquear indiscriminadamente el protocolo.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar ICMP para realizar reconocimiento, comprobar disponibilidad de sistemas o transportar comunicaciones maliciosas en determinados escenarios.


## TTL

**¿Qué es?**  
Time To Live es un valor de los paquetes IP que limita cuántos saltos de red puede realizar un paquete antes de ser descartado.

**¿Dónde lo encuentro?**  
En encabezados IP, routers, capturas de tráfico y herramientas de diagnóstico de red.

**¿Por qué me afecta?**  
Su análisis puede proporcionar información sobre rutas y ayudar a identificar determinadas anomalías en el tráfico.

**¿Cómo se soluciona?**  
Monitorear valores y patrones anómalos cuando sean relevantes y configurar correctamente los dispositivos de red.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría analizar valores TTL para obtener información sobre rutas o características de los sistemas y dispositivos de red.


## MTU

**¿Qué es?**  
Maximum Transmission Unit es el tamaño máximo de una unidad de datos que puede transmitirse por una interfaz de red sin fragmentación a ese nivel.

**¿Dónde lo encuentro?**  
En interfaces de red, routers, switches, sistemas operativos y configuraciones de redes físicas o virtuales.

**¿Por qué me afecta?**  
Una MTU incorrecta puede provocar fragmentación, pérdida de paquetes o problemas de conectividad y puede afectar determinadas comunicaciones.

**¿Cómo se soluciona?**  
Configurar valores de MTU compatibles entre los segmentos involucrados y verificar la ruta de red cuando existan problemas de fragmentación.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar comportamientos relacionados con fragmentación o tamaños de paquetes para intentar evadir determinados controles de red.
