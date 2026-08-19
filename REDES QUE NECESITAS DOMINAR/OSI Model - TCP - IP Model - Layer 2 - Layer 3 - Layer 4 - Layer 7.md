
## OSI Model

**¿Qué es?**  
El OSI Model (Open Systems Interconnection) es un modelo conceptual de siete capas utilizado para describir cómo se comunican los sistemas en una red.

**¿Dónde lo encuentro?**  
En diseño y troubleshooting de redes, documentación técnica, análisis de tráfico y formación en networking y ciberseguridad.

**¿Por qué me afecta?**  
Permite ubicar protocolos, dispositivos y problemas de seguridad dentro de una capa específica, facilitando el análisis de incidentes y comunicaciones.

**¿Cómo se soluciona?**  
Utilizando el modelo como referencia para analizar problemas y aplicar controles de seguridad en las diferentes capas de la comunicación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar debilidades en diferentes capas, desde ataques contra la infraestructura de red hasta vulnerabilidades en aplicaciones.

## TCP

**¿Qué es?**  
TCP (Transmission Control Protocol) es un protocolo de transporte orientado a conexión que proporciona entrega ordenada y confiable de datos entre dispositivos.

**¿Dónde lo encuentro?**  
En servicios como HTTP/HTTPS, SSH, SMTP, SMB y muchas otras aplicaciones que requieren comunicaciones confiables.

**¿Por qué me afecta?**  
Las conexiones TCP permiten identificar servicios y patrones de comunicación que pueden ser relevantes para detectar reconocimiento, acceso no autorizado o C2.

**¿Cómo se soluciona?**  
Restringiendo servicios TCP innecesarios, aplicando reglas de firewall y monitoreando conexiones y puertos expuestos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar TCP para realizar escaneos, conectarse a servicios vulnerables o establecer canales de comunicación con sistemas comprometidos.

## IP Model

**¿Qué es?**  
El IP Model es un modelo de referencia basado en las capas utilizadas por la arquitectura TCP/IP para describir cómo se transmiten los datos entre sistemas conectados en red.

**¿Dónde lo encuentro?**  
En redes modernas, configuraciones de infraestructura, protocolos de comunicación y análisis de tráfico.

**¿Por qué me afecta?**  
Ayuda a comprender cómo interactúan protocolos y dispositivos de red, facilitando el análisis de comunicaciones y posibles ataques.

**¿Cómo se soluciona?**  
Aplicando controles de seguridad adecuados a las diferentes capas, incluyendo segmentación, filtrado, autenticación y protección de aplicaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar debilidades en protocolos o servicios de diferentes capas para obtener acceso, interceptar comunicaciones o afectar sistemas.

## Layer 2

**¿Qué es?**  
Layer 2 es la capa de enlace de datos del modelo OSI y se encarga de la comunicación entre dispositivos dentro de una red local mediante mecanismos como Ethernet y direcciones MAC.

**¿Dónde lo encuentro?**  
En switches, tarjetas de red, redes Ethernet, VLAN y protocolos utilizados para la comunicación dentro de una LAN.

**¿Por qué me afecta?**  
Los ataques en esta capa pueden permitir interceptar tráfico, suplantar dispositivos o manipular comunicaciones dentro de una red local.

**¿Cómo se soluciona?**  
Utilizando segmentación mediante VLAN, controles de acceso, seguridad de puertos y mecanismos de protección contra ataques de capa 2.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar técnicas como MAC spoofing o ARP spoofing para manipular la comunicación dentro de una red local.

## Layer 3

**¿Qué es?**  
Layer 3 es la capa de red del modelo OSI y se encarga del direccionamiento lógico y el enrutamiento de paquetes entre diferentes redes.

**¿Dónde lo encuentro?**  
En routers, firewalls, protocolos IP y configuraciones de direccionamiento y enrutamiento.

**¿Por qué me afecta?**  
Las decisiones de enrutamiento y las reglas de esta capa determinan qué redes y sistemas pueden comunicarse entre sí.

**¿Cómo se soluciona?**  
Aplicando segmentación, filtrado de tráfico, rutas seguras y reglas de firewall correctamente configuradas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar reconocimiento de redes, aprovechar rutas o acceder a sistemas mediante servicios expuestos entre diferentes segmentos.

## Layer 4

**¿Qué es?**  
Layer 4 es la capa de transporte del modelo OSI y gestiona la comunicación entre aplicaciones mediante protocolos como TCP y UDP.

**¿Dónde lo encuentro?**  
En puertos de red, firewalls, sistemas operativos, servidores y aplicaciones que utilizan TCP o UDP.

**¿Por qué me afecta?**  
Los puertos y servicios expuestos en esta capa representan una parte importante de la superficie de ataque de un sistema.

**¿Cómo se soluciona?**  
Cerrando puertos innecesarios, restringiendo servicios mediante firewalls y monitoreando conexiones sospechosas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede escanear puertos para identificar servicios disponibles y posteriormente intentar explotarlos.

## Layer 7

**¿Qué es?**  
Layer 7 es la capa de aplicación del modelo OSI y corresponde a los servicios y protocolos con los que interactúan directamente las aplicaciones.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, correo electrónico, DNS y otros servicios que procesan datos destinados a aplicaciones.

**¿Por qué me afecta?**  
Las vulnerabilidades de aplicaciones pueden permitir ataques como inyección, autenticación incorrecta o ejecución de acciones no autorizadas.

**¿Cómo se soluciona?**  
Aplicando desarrollo seguro, validación de entradas, autenticación, autorización, WAF cuando corresponda y monitoreo de las aplicaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enviar solicitudes maliciosas para explotar vulnerabilidades de aplicaciones, robar información o ejecutar acciones no autorizadas.
