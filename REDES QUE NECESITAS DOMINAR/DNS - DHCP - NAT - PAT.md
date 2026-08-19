
## DNS

**¿Qué es?**  
DNS (Domain Name System) es un sistema que traduce nombres de dominio, como `example.com`, a direcciones IP y permite localizar servicios dentro de una red.

**¿Dónde lo encuentro?**  
En servidores DNS, routers, sistemas operativos, redes empresariales y servicios de Internet.

**¿Por qué me afecta?**  
DNS es fundamental para la comunicación de red y puede proporcionar información útil para detectar dominios maliciosos, consultas anómalas o actividad de C2.

**¿Cómo se soluciona?**  
Protegiendo los servidores DNS, controlando las consultas, aplicando filtrado y monitoreando dominios y patrones de resolución sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar DNS para realizar reconocimiento, comunicarse con infraestructura C2 o extraer información mediante técnicas como DNS tunneling.

## DHCP

**¿Qué es?**  
DHCP (Dynamic Host Configuration Protocol) asigna automáticamente parámetros de configuración de red, como direcciones IP, gateway y servidores DNS, a los dispositivos.

**¿Dónde lo encuentro?**  
En redes empresariales, routers, servidores y dispositivos que necesitan configuración automática para conectarse a una red.

**¿Por qué me afecta?**  
Un servidor DHCP no autorizado puede proporcionar configuraciones maliciosas y redirigir el tráfico de los dispositivos conectados.

**¿Cómo se soluciona?**  
Utilizando controles como DHCP Snooping, restringiendo quién puede proporcionar servicios DHCP y monitoreando asignaciones anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede desplegar un servidor DHCP malicioso para asignar un gateway o DNS controlado por él y manipular el tráfico de los dispositivos.

## NAT

**¿Qué es?**  
NAT (Network Address Translation) es una técnica que modifica direcciones IP en los paquetes para permitir la comunicación entre redes con diferentes espacios de direccionamiento.

**¿Dónde lo encuentro?**  
En routers, firewalls, gateways y redes donde se utilizan direcciones privadas para acceder a redes externas.

**¿Por qué me afecta?**  
NAT puede ocultar la estructura de direccionamiento interno, pero una configuración incorrecta puede exponer servicios internos mediante reglas de traducción.

**¿Cómo se soluciona?**  
Configurando correctamente las reglas de traducción, restringiendo conexiones entrantes y utilizando firewall y segmentación como controles complementarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar reglas de NAT o port forwarding mal configuradas para acceder desde el exterior a servicios internos.

## PAT

**¿Qué es?**  
PAT (Port Address Translation) es una forma de NAT que permite que múltiples dispositivos compartan una misma dirección IP utilizando diferentes números de puerto para distinguir sus conexiones.

**¿Dónde lo encuentro?**  
En routers, firewalls y gateways que permiten que múltiples dispositivos de una red privada compartan una dirección IPv4 pública.

**¿Por qué me afecta?**  
Una configuración incorrecta de PAT puede exponer servicios internos o dificultar la identificación del dispositivo interno responsable de una conexión.

**¿Cómo se soluciona?**  
Limitando las reglas de traducción y port forwarding, registrando las conexiones y aplicando controles de firewall adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar puertos publicados mediante PAT para acceder a servicios internos que no deberían estar expuestos a Internet.
