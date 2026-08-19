
## Port

**¿Qué es?**  
Un Port es un identificador numérico utilizado por los protocolos de transporte para dirigir comunicaciones hacia un servicio o proceso específico en un dispositivo.

**¿Dónde lo encuentro?**  
En firewalls, servidores, endpoints, escáneres de red y registros de conexiones como `TCP/443` o `UDP/53`.

**¿Por qué me afecta?**  
Los puertos expuestos pueden revelar servicios disponibles y aumentar la superficie de ataque si están innecesariamente accesibles o mal configurados.

**¿Cómo se soluciona?**  
Cerrando puertos innecesarios, restringiendo el acceso mediante firewalls y monitoreando servicios expuestos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede escanear puertos para identificar servicios vulnerables y utilizarlos como posibles puntos de entrada.

## TCP

**¿Qué es?**  
TCP (Transmission Control Protocol) es un protocolo de transporte orientado a conexión que proporciona entrega ordenada y confiable de datos entre dispositivos.

**¿Dónde lo encuentro?**  
En servicios como HTTP/HTTPS, SSH, correo electrónico, bases de datos y muchas otras comunicaciones de red.

**¿Por qué me afecta?**  
Las conexiones TCP pueden revelar servicios accesibles y patrones de comunicación útiles para detectar reconocimiento o actividad sospechosa.

**¿Cómo se soluciona?**  
Restringiendo los servicios TCP innecesarios, aplicando reglas de firewall y monitoreando conexiones y puertos expuestos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar conexiones TCP para escanear servicios, conectarse a sistemas vulnerables o establecer comunicaciones con infraestructura maliciosa.

## UDP

**¿Qué es?**  
UDP (User Datagram Protocol) es un protocolo de transporte que permite enviar datagramas sin establecer una conexión y sin garantizar su entrega o su orden.

**¿Dónde lo encuentro?**  
En servicios como DNS, DHCP, VoIP, streaming y otras aplicaciones que utilizan comunicaciones rápidas sin las garantías de TCP.

**¿Por qué me afecta?**  
Los servicios UDP expuestos pueden presentar riesgos y determinados patrones de tráfico UDP pueden ser relevantes durante una investigación.

**¿Cómo se soluciona?**  
Limitando los servicios UDP necesarios, aplicando reglas de firewall y monitoreando tráfico inusual o inesperado.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar servicios UDP expuestos para realizar reconocimiento, explotar servicios vulnerables o establecer determinados canales de comunicación.

## ICMP

**¿Qué es?**  
ICMP (Internet Control Message Protocol) es un protocolo utilizado para enviar mensajes de control, diagnóstico y errores relacionados con las comunicaciones IP.

**¿Dónde lo encuentro?**  
En herramientas como `ping`, mecanismos de diagnóstico de red, routers, firewalls y registros de tráfico.

**¿Por qué me afecta?**  
El tráfico ICMP puede proporcionar información sobre dispositivos disponibles y, en determinados escenarios, utilizarse para transportar o señalizar actividad maliciosa.

**¿Cómo se soluciona?**  
Controlando los tipos de mensajes ICMP permitidos mediante firewalls y monitoreando patrones anómalos sin bloquear indiscriminadamente el protocolo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar ICMP para reconocimiento, identificar hosts activos o, en determinados ataques, transportar información mediante técnicas de tunneling.

## ARP

**¿Qué es?**  
ARP (Address Resolution Protocol) permite asociar una dirección IPv4 con la dirección MAC correspondiente dentro de una red local.

**¿Dónde lo encuentro?**  
En redes Ethernet, tablas ARP de dispositivos, switches, sistemas operativos y herramientas de diagnóstico de red.

**¿Por qué me afecta?**  
ARP no proporciona autenticación nativa, por lo que puede ser utilizado para manipular la asociación entre direcciones IP y MAC dentro de una red local.

**¿Cómo se soluciona?**  
Utilizando controles como Dynamic ARP Inspection cuando estén disponibles, segmentación de red y monitoreo de cambios o anomalías en las tablas ARP.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar ARP spoofing o ARP poisoning para asociar su dirección MAC con la IP de otro dispositivo y facilitar ataques como Man-in-the-Middle.
