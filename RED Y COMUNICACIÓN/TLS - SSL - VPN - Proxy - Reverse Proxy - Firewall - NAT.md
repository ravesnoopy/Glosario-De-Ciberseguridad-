
## TLS

**¿Qué es?**  
TLS (Transport Layer Security) es un protocolo criptográfico que protege las comunicaciones mediante cifrado, autenticación e integridad de los datos.

**¿Dónde lo encuentro?**  
En HTTPS, correo electrónico, APIs, VPN y otros servicios que requieren comunicaciones protegidas.

**¿Por qué me afecta?**  
Protege información durante su transmisión y reduce el riesgo de interceptación o modificación de las comunicaciones.

**¿Cómo se soluciona?**  
Utilizando versiones modernas de TLS, certificados válidos y configuraciones criptográficas seguras, evitando protocolos y algoritmos obsoletos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar configuraciones TLS débiles, certificados comprometidos o tráfico cifrado para dificultar la inspección de sus comunicaciones.

## SSL

**¿Qué es?**  
SSL (Secure Sockets Layer) fue una familia de protocolos criptográficos utilizada para proteger comunicaciones de red y es el predecesor de TLS.

**¿Dónde lo encuentro?**  
En documentación antigua, configuraciones heredadas y servicios que todavía utilizan el término "SSL" para referirse genéricamente al cifrado TLS.

**¿Por qué me afecta?**  
Las versiones antiguas de SSL presentan vulnerabilidades conocidas y no deben utilizarse para proteger comunicaciones actuales.

**¿Cómo se soluciona?**  
Deshabilitando SSLv2 y SSLv3 y utilizando versiones modernas de TLS con configuraciones criptográficas seguras.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar protocolos SSL obsoletos o configuraciones inseguras para interceptar o manipular comunicaciones.

## VPN

**¿Qué es?**  
VPN (Virtual Private Network) es una tecnología que crea un canal protegido para transportar tráfico entre dispositivos o redes a través de una infraestructura de red no confiable.

**¿Dónde lo encuentro?**  
En acceso remoto empresarial, conexiones entre oficinas, dispositivos de usuarios y servicios que requieren acceso protegido a redes privadas.

**¿Por qué me afecta?**  
Una VPN mal configurada o con credenciales comprometidas puede proporcionar a un atacante acceso directo a recursos internos.

**¿Cómo se soluciona?**  
Utilizando autenticación fuerte, MFA, protocolos seguros, segmentación de acceso, gestión de parches y monitoreo de conexiones VPN.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales robadas para conectarse a una VPN legítima y utilizarla como punto de entrada a la red interna.

## Proxy

**¿Qué es?**  
Un Proxy es un servidor intermediario que recibe solicitudes de un cliente y las reenvía hacia otro servicio o destino.

**¿Dónde lo encuentro?**  
En redes corporativas, gateways de Internet, sistemas de filtrado web y arquitecturas donde se controla o inspecciona el tráfico de los usuarios.

**¿Por qué me afecta?**  
Puede controlar el acceso a Internet y registrar tráfico, pero una configuración incorrecta puede permitir conexiones no autorizadas o dificultar la visibilidad.

**¿Cómo se soluciona?**  
Aplicando reglas de acceso, autenticación, filtrado, registro y monitoreo adecuado del tráfico que atraviesa el proxy.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar utilizar proxies para ocultar el origen de sus conexiones o comunicarse con infraestructura externa.

## Reverse Proxy

**¿Qué es?**  
Un Reverse Proxy es un servidor intermediario que recibe solicitudes de clientes y las dirige hacia uno o más servidores backend.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, balanceadores de carga y arquitecturas donde los servidores internos no se exponen directamente a Internet.

**¿Por qué me afecta?**  
Una configuración insegura puede exponer servicios internos, permitir ataques contra aplicaciones o proporcionar información sobre la infraestructura backend.

**¿Cómo se soluciona?**  
Aplicando controles de acceso, TLS, filtrado, validación de solicitudes, actualización del software y segmentación entre el proxy y los servidores internos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar vulnerabilidades del reverse proxy o manipular solicitudes para acceder a recursos internos que deberían estar protegidos.

## Firewall

**¿Qué es?**  
Un Firewall es un mecanismo de seguridad que controla el tráfico de red según reglas definidas para permitir o bloquear comunicaciones.

**¿Dónde lo encuentro?**  
En redes empresariales, servidores, endpoints, routers, servicios cloud y puntos de conexión entre diferentes segmentos de red.

**¿Por qué me afecta?**  
Ayuda a reducir la superficie de ataque al controlar qué sistemas, servicios y redes pueden comunicarse entre sí.

**¿Cómo se soluciona?**  
Aplicando reglas de mínimo privilegio, segmentación, revisión periódica de políticas y monitoreo de tráfico bloqueado y permitido.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar servicios permitidos, explotar reglas demasiado amplias o utilizar tráfico autorizado para intentar evadir los controles de red.

## NAT

**¿Qué es?**  
NAT (Network Address Translation) es una técnica que modifica direcciones IP en los paquetes para permitir, entre otros usos, que múltiples dispositivos privados compartan direcciones públicas.

**¿Dónde lo encuentro?**  
En routers, firewalls, gateways y redes donde existen direcciones privadas y conexiones hacia redes externas.

**¿Por qué me afecta?**  
NAT puede ocultar la estructura interna de una red frente a Internet, pero no sustituye controles de seguridad como un firewall.

**¿Cómo se soluciona?**  
Configurando correctamente las reglas de traducción, restringiendo conexiones entrantes y utilizando controles adicionales de segmentación y firewall.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar reglas de NAT o port forwarding mal configuradas para alcanzar servicios internos desde redes externas.
