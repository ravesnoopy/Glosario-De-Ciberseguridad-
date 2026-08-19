
## Private IP

**¿Qué es?**  
Una Private IP es una dirección utilizada dentro de redes privadas y no se enruta directamente a través de Internet.

**¿Dónde lo encuentro?**  
En redes internas de empresas, hogares, servidores, estaciones de trabajo, dispositivos IoT y entornos cloud.

**¿Por qué me afecta?**  
Permite organizar redes internas, pero una configuración o exposición incorrecta puede permitir que sistemas internos sean accesibles desde redes no autorizadas.

**¿Cómo se soluciona?**  
Utilizando segmentación, firewalls, controles de acceso y configuraciones adecuadas de NAT cuando los sistemas necesiten comunicarse con Internet.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar descubrir direcciones privadas mediante reconocimiento interno después de obtener acceso a la red.

## Public IP

**¿Qué es?**  
Una Public IP es una dirección IP enrutable en Internet que puede utilizarse para identificar un dispositivo o servicio accesible desde redes externas.

**¿Dónde lo encuentro?**  
En servidores públicos, firewalls, routers, servicios cloud y aplicaciones expuestas a Internet.

**¿Por qué me afecta?**  
Un servicio asociado a una Public IP puede quedar expuesto a escaneos, explotación y ataques provenientes de Internet.

**¿Cómo se soluciona?**  
Reduciendo servicios expuestos, utilizando firewalls, controles de acceso, segmentación y monitoreo del tráfico entrante.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede escanear una Public IP para identificar puertos y servicios vulnerables accesibles desde Internet.

## RFC1918

**¿Qué es?**  
RFC1918 define tres rangos de direcciones IPv4 reservadas para redes privadas: `10.0.0.0/8`, `172.16.0.0/12` y `192.168.0.0/16`.

**¿Dónde lo encuentro?**  
En redes internas, routers, firewalls, servidores, estaciones de trabajo y configuraciones de infraestructura privada.

**¿Por qué me afecta?**  
Estos rangos permiten separar el direccionamiento interno del espacio público de Internet y son fundamentales para diseñar redes privadas.

**¿Cómo se soluciona?**  
Planificando correctamente los rangos privados, evitando solapamientos entre redes y aplicando segmentación y controles de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras obtener acceso interno, puede realizar reconocimiento de rangos RFC1918 para identificar otros sistemas y segmentos disponibles.

## VLAN

**¿Qué es?**  
Una VLAN (Virtual Local Area Network) es una segmentación lógica de una red que permite separar dispositivos en diferentes dominios de broadcast utilizando infraestructura física compartida.

**¿Dónde lo encuentro?**  
En switches, redes empresariales, centros de datos y entornos donde se requiere separar usuarios, servidores u otros dispositivos.

**¿Por qué me afecta?**  
Una segmentación VLAN adecuada puede limitar el movimiento lateral y reducir el alcance de un compromiso.

**¿Cómo se soluciona?**  
Separando recursos según su función, restringiendo la comunicación entre VLAN mediante controles de capa 3 y protegiendo la configuración de los switches.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar realizar VLAN hopping o aprovechar configuraciones incorrectas para acceder a segmentos que deberían estar aislados.

## Routing

**¿Qué es?**  
Routing es el proceso mediante el cual los dispositivos de red determinan cómo enviar paquetes desde una red de origen hacia una red de destino.

**¿Dónde lo encuentro?**  
En routers, firewalls, switches de capa 3 y configuraciones de redes empresariales y cloud.

**¿Por qué me afecta?**  
Las rutas determinan qué redes pueden comunicarse entre sí y una configuración incorrecta puede crear accesos no deseados.

**¿Cómo se soluciona?**  
Aplicando rutas correctamente definidas, segmentación, controles de acceso y monitoreo de cambios en la infraestructura de enrutamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar rutas mal configuradas para alcanzar redes internas o intentar manipular el tráfico mediante ataques contra la infraestructura de enrutamiento.

## Switching

**¿Qué es?**  
Switching es el proceso de reenviar tramas dentro de una red local mediante switches, utilizando principalmente direcciones MAC para determinar el destino.

**¿Dónde lo encuentro?**  
En switches de red, redes Ethernet, centros de datos y redes LAN empresariales.

**¿Por qué me afecta?**  
Una infraestructura de switching comprometida puede permitir interceptación, manipulación de tráfico o acceso no autorizado a segmentos de red.

**¿Cómo se soluciona?**  
Aplicando VLAN, port security, autenticación de acceso, protección contra ataques de capa 2 y monitoreo de la infraestructura.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar manipular tablas MAC, realizar ataques de capa 2 o conectarse a puertos de red no protegidos.

## Proxy

**¿Qué es?**  
Un Proxy es un servidor intermediario que recibe solicitudes de un cliente y las reenvía hacia otro servidor o servicio.

**¿Dónde lo encuentro?**  
En redes corporativas, gateways de Internet, sistemas de filtrado web y arquitecturas donde se controla el tráfico de los usuarios.

**¿Por qué me afecta?**  
Puede proporcionar filtrado, registro y control del tráfico, pero una configuración incorrecta puede permitir conexiones no autorizadas o reducir la visibilidad de las comunicaciones.

**¿Cómo se soluciona?**  
Aplicando autenticación, filtrado, reglas de acceso, registro y monitoreo del tráfico que atraviesa el proxy.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar proxies para ocultar el origen de sus conexiones o intentar evadir controles de red.

## Reverse Proxy

**¿Qué es?**  
Un Reverse Proxy es un servidor intermediario que recibe solicitudes externas y las reenvía a uno o más servidores backend internos.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, balanceadores de carga y arquitecturas donde los servidores backend no se exponen directamente a Internet.

**¿Por qué me afecta?**  
Una configuración incorrecta puede exponer servicios internos, permitir solicitudes maliciosas o revelar información sobre la infraestructura backend.

**¿Cómo se soluciona?**  
Aplicando controles de acceso, TLS, validación de solicitudes, actualización del software, filtrado y segmentación entre el proxy y los servidores backend.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar vulnerabilidades del reverse proxy o manipular solicitudes para intentar acceder a recursos internos.

## VPN

**¿Qué es?**  
Una VPN (Virtual Private Network) crea un canal protegido para transportar tráfico entre dispositivos o redes a través de una infraestructura no confiable.

**¿Dónde lo encuentro?**  
En accesos remotos empresariales, conexiones entre oficinas, dispositivos de usuarios y servicios que requieren acceso protegido a redes privadas.

**¿Por qué me afecta?**  
Una VPN comprometida o mal configurada puede proporcionar acceso a recursos internos y convertirse en un punto de entrada para un atacante.

**¿Cómo se soluciona?**  
Utilizando MFA, autenticación fuerte, protocolos seguros, segmentación, gestión de parches y monitoreo de conexiones VPN.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para acceder a una VPN legítima y utilizarla como punto de entrada a la red interna.
