
## Packet

**¿Qué es?**  
Unidad de datos utilizada en la capa de red para transportar información entre dispositivos, incluyendo datos y encabezados necesarios para su entrega.

**¿Dónde lo encuentro?**  
En redes IP, routers, firewalls, capturas de tráfico y herramientas de análisis como Wireshark.

**¿Por qué me afecta?**  
El análisis de paquetes permite identificar comunicaciones, conexiones sospechosas, errores y posibles actividades maliciosas en una red.

**¿Cómo se soluciona?**  
Monitorear el tráfico, aplicar segmentación y controles de red y analizar paquetes sospechosos cuando sea necesario.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría analizar o generar tráfico de red para realizar reconocimiento, comunicarse con sistemas comprometidos o intentar evadir controles.


## Frame

**¿Qué es?**  
Unidad de datos utilizada principalmente en la capa de enlace de datos para transportar información dentro de una red local.

**¿Dónde lo encuentro?**  
En redes Ethernet, switches, adaptadores de red y capturas de tráfico a nivel de enlace.

**¿Por qué me afecta?**  
El análisis de frames permite identificar comunicaciones dentro de una red local y detectar comportamientos anómalos o ataques de capa 2.

**¿Cómo se soluciona?**  
Aplicar segmentación, controles de acceso de red y mecanismos de seguridad en switches y dispositivos de infraestructura.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría manipular o generar tráfico de capa 2 para realizar reconocimiento, interceptar comunicaciones o afectar el funcionamiento de la red.


## Broadcast

**¿Qué es?**  
Método de comunicación en el que un dispositivo envía datos destinados a todos los dispositivos dentro de un dominio de broadcast.

**¿Dónde lo encuentro?**  
Principalmente en redes locales, donde determinados protocolos utilizan mensajes dirigidos a múltiples dispositivos simultáneamente.

**¿Por qué me afecta?**  
Un exceso de tráfico broadcast puede degradar la red y determinados ataques pueden aprovechar este comportamiento para afectar o descubrir dispositivos.

**¿Cómo se soluciona?**  
Segmentar redes, controlar el tráfico broadcast y utilizar configuraciones adecuadas en switches y dispositivos de red.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar grandes cantidades de tráfico broadcast para degradar el rendimiento o utilizarlo para obtener información sobre dispositivos de la red.


## Unicast

**¿Qué es?**  
Método de comunicación en el que los datos se envían desde un origen hacia un único destino específico.

**¿Dónde lo encuentro?**  
En la mayoría de las comunicaciones normales entre dispositivos, servidores, aplicaciones y servicios de red.

**¿Por qué me afecta?**  
El análisis del tráfico unicast permite identificar conexiones entre sistemas y detectar comunicaciones inesperadas o potencialmente maliciosas.

**¿Cómo se soluciona?**  
Controlar las comunicaciones mediante firewalls, segmentación, listas de acceso y monitoreo de tráfico.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría establecer conexiones unicast con sistemas comprometidos para realizar reconocimiento, transferencia de datos o comunicación con infraestructura externa.


## Multicast

**¿Qué es?**  
Método de comunicación en el que un dispositivo envía datos a un grupo específico de receptores interesados en recibirlos.

**¿Dónde lo encuentro?**  
En redes que utilizan servicios como distribución de contenido, streaming, descubrimiento de servicios y determinadas aplicaciones empresariales.

**¿Por qué me afecta?**  
Una configuración incorrecta puede generar tráfico innecesario o permitir que dispositivos reciban comunicaciones que no deberían alcanzarles.

**¿Cómo se soluciona?**  
Controlar los grupos multicast, configurar correctamente la infraestructura de red y limitar el tráfico a los segmentos necesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría abusar de servicios multicast o generar tráfico excesivo para obtener información o afectar el rendimiento de determinados segmentos de red.
