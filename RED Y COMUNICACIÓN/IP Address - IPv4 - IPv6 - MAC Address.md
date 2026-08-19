
## IP Address

**¿Qué es?**  
Una IP Address es un identificador lógico asignado a una interfaz de red para permitir la comunicación entre dispositivos dentro de una red o entre redes.

**¿Dónde lo encuentro?**  
En endpoints, servidores, routers, firewalls, logs, configuraciones de red y registros de conexiones.

**¿Por qué me afecta?**  
Las direcciones IP permiten identificar el origen y destino del tráfico y pueden utilizarse para investigar conexiones sospechosas o controlar el acceso a recursos.

**¿Cómo se soluciona?**  
Gestionando correctamente el direccionamiento, segmentando redes, aplicando reglas de firewall y monitoreando el tráfico asociado a las direcciones IP.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar una IP comprometida, falsificada o controlada por él para comunicarse con sistemas objetivo o establecer infraestructura maliciosa.

## IPv4

**¿Qué es?**  
IPv4 es la cuarta versión del Protocolo de Internet y utiliza direcciones de 32 bits para identificar interfaces dentro de una red.

**¿Dónde lo encuentro?**  
En prácticamente cualquier entorno de red que utilice IPv4, incluyendo endpoints, servidores, routers, firewalls y dispositivos de red.

**¿Por qué me afecta?**  
Las direcciones IPv4 aparecen constantemente en registros y tráfico de red, por lo que son importantes para identificar comunicaciones y posibles indicadores de compromiso.

**¿Cómo se soluciona?**  
Utilizando direccionamiento adecuado, segmentación, controles de firewall, NAT cuando corresponda y monitoreo del tráfico IPv4.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar direcciones IPv4 para realizar reconocimiento, conectarse a servicios expuestos, establecer C2 o comunicarse con sistemas comprometidos.

## IPv6

**¿Qué es?**  
IPv6 es la versión más reciente del Protocolo de Internet y utiliza direcciones de 128 bits para proporcionar un espacio de direccionamiento mucho mayor que IPv4.

**¿Dónde lo encuentro?**  
En sistemas operativos, redes empresariales, proveedores de Internet, dispositivos modernos y entornos que soportan direccionamiento IPv6.

**¿Por qué me afecta?**  
Una red que no monitorea o protege IPv6 adecuadamente puede generar una superficie de ataque adicional y permitir tráfico que no esté contemplado en los controles IPv4.

**¿Cómo se soluciona?**  
Configurando correctamente IPv6, aplicando controles equivalentes a los utilizados para IPv4 y monitoreando su tráfico y servicios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar configuraciones IPv6 débiles, servicios expuestos o controles de seguridad que no inspeccionen adecuadamente el tráfico IPv6.

## MAC Address

**¿Qué es?**  
Una MAC Address es un identificador asociado a una interfaz de red utilizado principalmente para la comunicación dentro de una red local.

**¿Dónde lo encuentro?**  
En tarjetas de red, switches, tablas ARP, configuraciones de dispositivos, herramientas de administración y registros de red local.

**¿Por qué me afecta?**  
Puede ayudar a identificar dispositivos dentro de una red local y relacionar actividad de red con un equipo específico.

**¿Cómo se soluciona?**  
Monitoreando las tablas de red, utilizando controles de acceso como port security cuando corresponda y correlacionando MAC con otros identificadores del dispositivo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar MAC spoofing para hacerse pasar por otro dispositivo o evadir determinados controles basados únicamente en la dirección MAC.
