
## Ethernet

**¿Qué es?**  
Ethernet es una tecnología de red utilizada para transmitir datos entre dispositivos dentro de una red local mediante medios físicos o inalámbricos compatibles.

**¿Dónde lo encuentro?**  
En redes LAN, switches, tarjetas de red, cables Ethernet y dispositivos conectados a una infraestructura de red.

**¿Por qué me afecta?**  
Una red Ethernet comprometida puede permitir que un atacante intercepte, manipule o redirija tráfico dentro de la red local.

**¿Cómo se soluciona?**  
Aplicando segmentación, controles de acceso, seguridad de puertos, monitoreo de tráfico y configuraciones seguras en switches y dispositivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar el acceso a la red local para realizar reconocimiento, manipular tráfico o intentar ataques contra otros dispositivos.

## MAC

**¿Qué es?**  
MAC (Media Access Control) es una dirección asociada a una interfaz de red y utilizada principalmente para identificar dispositivos dentro de una red local.

**¿Dónde lo encuentro?**  
En tarjetas de red, switches, tablas ARP, configuraciones de dispositivos y registros de infraestructura de red.

**¿Por qué me afecta?**  
Puede ayudar a identificar dispositivos y relacionar actividad de red con un equipo específico, pero no debe considerarse una identidad segura por sí sola.

**¿Cómo se soluciona?**  
Utilizando controles como port security, segmentación y autenticación de acceso a la red cuando estén disponibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar MAC spoofing para hacerse pasar por otro dispositivo o intentar evadir controles basados únicamente en la dirección MAC.

## ARP

**¿Qué es?**  
ARP (Address Resolution Protocol) permite asociar una dirección IPv4 con la dirección MAC correspondiente dentro de una red local.

**¿Dónde lo encuentro?**  
En redes Ethernet, tablas ARP, sistemas operativos, switches y herramientas de diagnóstico de red.

**¿Por qué me afecta?**  
ARP no proporciona autenticación nativa, por lo que puede ser manipulado para alterar la asociación entre direcciones IP y MAC.

**¿Cómo se soluciona?**  
Utilizando controles como Dynamic ARP Inspection, segmentación y monitoreo de cambios anómalos en las tablas ARP.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar ARP spoofing o ARP poisoning para redirigir tráfico a través de su dispositivo y facilitar un ataque Man-in-the-Middle.

## IP

**¿Qué es?**  
IP (Internet Protocol) es el protocolo encargado de direccionar y enrutar paquetes entre dispositivos y redes mediante direcciones IP.

**¿Dónde lo encuentro?**  
En prácticamente todas las comunicaciones de red, incluyendo endpoints, servidores, routers, firewalls y dispositivos conectados a Internet.

**¿Por qué me afecta?**  
Las direcciones IP permiten identificar los extremos de una comunicación y son fundamentales para analizar tráfico, investigar incidentes y aplicar controles de acceso.

**¿Cómo se soluciona?**  
Utilizando direccionamiento adecuado, segmentación, reglas de firewall y monitoreo del tráfico IP.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar direcciones IP para realizar reconocimiento, identificar servicios expuestos o comunicarse con sistemas comprometidos.

## IPv4

**¿Qué es?**  
IPv4 es la cuarta versión del Protocolo de Internet y utiliza direcciones de 32 bits para identificar interfaces de red.

**¿Dónde lo encuentro?**  
En endpoints, servidores, routers, firewalls y prácticamente cualquier red que utilice el protocolo IPv4.

**¿Por qué me afecta?**  
Las direcciones IPv4 aparecen constantemente en registros y tráfico de red, por lo que son importantes para identificar comunicaciones y posibles indicadores de compromiso.

**¿Cómo se soluciona?**  
Utilizando direccionamiento y segmentación adecuados, controles de firewall y monitoreo del tráfico IPv4.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar direcciones IPv4 para realizar reconocimiento, conectarse a servicios vulnerables o establecer comunicaciones con infraestructura maliciosa.

## IPv6

**¿Qué es?**  
IPv6 es la versión más reciente del Protocolo de Internet y utiliza direcciones de 128 bits para proporcionar un espacio de direccionamiento mucho mayor que IPv4.

**¿Dónde lo encuentro?**  
En sistemas operativos, redes empresariales, proveedores de Internet, dispositivos modernos y entornos que soportan IPv6.

**¿Por qué me afecta?**  
Una red que no protege o monitorea IPv6 adecuadamente puede crear una superficie de ataque adicional fuera de los controles configurados para IPv4.

**¿Cómo se soluciona?**  
Configurando correctamente IPv6, aplicando controles equivalentes a los utilizados para IPv4 y monitoreando su tráfico y servicios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar servicios IPv6 expuestos o controles de seguridad que no inspeccionen adecuadamente el tráfico IPv6.

## Subnet Mask

**¿Qué es?**  
Subnet Mask es un valor utilizado con IPv4 para determinar qué parte de una dirección corresponde a la red y qué parte identifica al host.

**¿Dónde lo encuentro?**  
En configuraciones de red, routers, servidores, endpoints y dispositivos que utilizan direccionamiento IPv4.

**¿Por qué me afecta?**  
Una máscara incorrecta puede provocar errores de segmentación, comunicación no deseada o una exposición mayor de la red.

**¿Cómo se soluciona?**  
Definiendo correctamente las subredes, verificando el direccionamiento y aplicando segmentación acorde con las necesidades de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar una segmentación deficiente para descubrir o comunicarse con más dispositivos de los que deberían estar accesibles.

## CIDR

**¿Qué es?**  
CIDR (Classless Inter-Domain Routing) es un método para representar rangos de direcciones IP mediante un prefijo que indica cuántos bits pertenecen a la red, como `192.168.1.0/24`.

**¿Dónde lo encuentro?**  
En configuraciones de redes, routers, firewalls, reglas de acceso, servicios cloud y documentación de infraestructura.

**¿Por qué me afecta?**  
Una definición incorrecta de rangos CIDR puede permitir acceso a más direcciones de las necesarias o generar una segmentación deficiente.

**¿Cómo se soluciona?**  
Definiendo rangos CIDR con precisión y aplicando el principio de mínimo acceso en reglas de red y firewall.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar rangos excesivamente amplios para alcanzar sistemas que no deberían estar accesibles desde su punto de origen.

## Default Gateway

**¿Qué es?**  
Default Gateway es el dispositivo de red al que un host envía los paquetes destinados a redes que no pertenecen a su propia subred.

**¿Dónde lo encuentro?**  
En configuraciones de red de endpoints, servidores, routers y otros dispositivos conectados a una red IP.

**¿Por qué me afecta?**  
Un gateway comprometido o configurado incorrectamente puede permitir redirigir tráfico, interrumpir comunicaciones o facilitar ataques de intermediario.

**¿Cómo se soluciona?**  
Protegiendo los dispositivos de red, controlando sus configuraciones y monitoreando cambios inesperados en los gateways utilizados por los hosts.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar manipular el gateway para redirigir tráfico hacia un sistema controlado por él o interrumpir la comunicación de los dispositivos.
