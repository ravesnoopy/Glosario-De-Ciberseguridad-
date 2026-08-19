
## TLS

**¿Qué es?**  
TLS (Transport Layer Security) es un protocolo criptográfico que protege las comunicaciones mediante cifrado, integridad de los datos y autenticación de las partes cuando corresponde.

**¿Dónde lo encuentro?**  
En conexiones HTTPS, correo electrónico, APIs, VPN y otros servicios que necesitan proteger datos mientras se transmiten por una red.

**¿Por qué me afecta?**  
Sin una protección adecuada, un atacante podría interceptar o manipular información durante su transmisión, especialmente en redes no confiables.

**¿Cómo se soluciona?**  
Utilizando versiones modernas de TLS, certificados válidos y configuraciones criptográficas seguras, deshabilitando protocolos y algoritmos obsoletos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar configuraciones débiles, protocolos obsoletos o certificados comprometidos para interceptar o manipular comunicaciones.

## SSL

**¿Qué es?**  
SSL (Secure Sockets Layer) fue una familia de protocolos utilizada para proteger comunicaciones mediante cifrado, pero actualmente está obsoleta y fue reemplazada por TLS.

**¿Dónde lo encuentro?**  
Puede aparecer en configuraciones, documentación o sistemas antiguos que todavía utilizan el término SSL para referirse a certificados o conexiones seguras.

**¿Por qué me afecta?**  
Las versiones antiguas de SSL contienen debilidades conocidas y no deben utilizarse para proteger comunicaciones actuales.

**¿Cómo se soluciona?**  
Deshabilitando SSL y utilizando versiones modernas de TLS con configuraciones criptográficas seguras.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar sistemas que todavía permiten protocolos SSL obsoletos para degradar o comprometer la seguridad de la comunicación.

## VPN

**¿Qué es?**  
VPN (Virtual Private Network) es una tecnología que crea un canal protegido entre dispositivos o redes para transportar tráfico a través de una infraestructura que puede no ser confiable.

**¿Dónde lo encuentro?**  
En conexiones de acceso remoto, redes corporativas, dispositivos de usuarios y servicios utilizados para conectar diferentes redes mediante Internet.

**¿Por qué me afecta?**  
Una VPN comprometida o mal configurada puede proporcionar a un atacante acceso a recursos internos que normalmente no están expuestos directamente a Internet.

**¿Cómo se soluciona?**  
Utilizando protocolos seguros, MFA, controles de acceso, actualizaciones, segmentación de red y monitoreo de los accesos VPN.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede atacar el servicio VPN, robar credenciales o aprovechar una vulnerabilidad para obtener acceso a la red interna.

## Proxy

**¿Qué es?**  
Un Proxy es un servidor intermediario que recibe solicitudes de un cliente y las reenvía hacia otro servidor en su nombre.

**¿Dónde lo encuentro?**  
En redes corporativas, sistemas de filtrado web, servidores de acceso a Internet y arquitecturas donde se requiere controlar o intermediar el tráfico.

**¿Por qué me afecta?**  
Un proxy puede controlar y registrar comunicaciones, pero una configuración incorrecta puede permitir accesos no autorizados o exponer información sobre la red.

**¿Cómo se soluciona?**  
Configurando correctamente las reglas de acceso, autenticación, filtrado, registros y permisos del servidor proxy.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar abusar de un proxy mal configurado para evadir controles, acceder a recursos internos o utilizarlo como intermediario para ocultar el origen de determinadas solicitudes.

## Reverse Proxy

**¿Qué es?**  
Un Reverse Proxy es un servidor intermediario que recibe solicitudes de los clientes y las dirige hacia uno o varios servidores backend.

**¿Dónde lo encuentro?**  
Delante de aplicaciones web, APIs y servidores de aplicaciones, especialmente en arquitecturas con balanceo de carga, caching o protección de servicios.

**¿Por qué me afecta?**  
Una configuración incorrecta puede exponer servidores internos, permitir el acceso a recursos no previstos o provocar errores en controles de autenticación y autorización.

**¿Cómo se soluciona?**  
Restringiendo los backends, configurando correctamente las rutas y cabeceras, aplicando controles de acceso y manteniendo actualizado el software.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar explotar configuraciones incorrectas del reverse proxy para acceder a servicios internos, evadir controles o manipular cómo se procesan las solicitudes.

## Firewall

**¿Qué es?**  
Un Firewall es un mecanismo de seguridad que controla el tráfico de red según reglas definidas para permitir o bloquear determinadas conexiones.

**¿Dónde lo encuentro?**  
En redes corporativas, servidores, dispositivos de red, sistemas operativos y entornos cloud.

**¿Por qué me afecta?**  
Un firewall correctamente configurado reduce la exposición de sistemas y limita las comunicaciones no autorizadas entre redes o dispositivos.

**¿Cómo se soluciona?**  
Aplicando reglas basadas en el principio de mínimo privilegio, eliminando accesos innecesarios, revisando periódicamente las reglas y registrando eventos relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar servicios permitidos, puertos expuestos o reglas demasiado permisivas para encontrar una vía de acceso o comunicarse con sistemas comprometidos.

## NAT

**¿Qué es?**  
NAT (Network Address Translation) es una técnica que modifica direcciones IP en los paquetes de red para permitir la comunicación entre redes con diferentes espacios de direccionamiento.

**¿Dónde lo encuentro?**  
En routers, firewalls y dispositivos de red que conectan redes privadas con Internet u otras redes.

**¿Por qué me afecta?**  
NAT puede ocultar direcciones privadas y facilitar el uso de direcciones IP compartidas, pero no debe considerarse un mecanismo de seguridad por sí mismo.

**¿Cómo se soluciona?**  
Configurando correctamente las reglas de traducción y combinándolas con firewalls, segmentación y controles de acceso adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar reglas de NAT o redirecciones de puertos mal configuradas para alcanzar servicios internos que no deberían estar expuestos.
