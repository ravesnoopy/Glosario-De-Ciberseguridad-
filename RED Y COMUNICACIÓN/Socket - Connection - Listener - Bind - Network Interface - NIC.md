
## Socket

**¿Qué es?**  
Punto lógico de comunicación que permite a un proceso enviar y recibir datos a través de una red, normalmente asociado con una dirección IP y un puerto.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones de red, servidores, herramientas de monitoreo y análisis de conexiones.

**¿Por qué me afecta?**  
Los sockets permiten identificar qué procesos están comunicándose y qué servicios de red están activos en un sistema.

**¿Cómo se soluciona?**  
Limitar servicios expuestos, aplicar firewalls, controlar puertos y monitorear sockets y conexiones inesperadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar sockets para establecer comunicaciones con servicios comprometidos o con infraestructura externa.


## Connection

**¿Qué es?**  
Comunicación establecida entre dos extremos de una red para intercambiar datos mediante un protocolo determinado.

**¿Dónde lo encuentro?**  
En aplicaciones, sistemas operativos, servidores, firewalls, routers y herramientas de monitoreo de red.

**¿Por qué me afecta?**  
Las conexiones permiten identificar comunicaciones legítimas y detectar accesos, conexiones externas o comportamientos sospechosos.

**¿Cómo se soluciona?**  
Controlar las conexiones mediante firewalls, segmentación, listas de acceso y monitoreo de tráfico.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría establecer conexiones con sistemas comprometidos para ejecutar acciones, transferir información o comunicarse con infraestructura de control.


## Listener

**¿Qué es?**  
Proceso o servicio que permanece esperando conexiones entrantes en una dirección de red y puerto determinados.

**¿Dónde lo encuentro?**  
En servidores, aplicaciones de red, servicios del sistema operativo y herramientas de monitoreo de conexiones.

**¿Por qué me afecta?**  
Un listener innecesario o expuesto puede aumentar la superficie de ataque y proporcionar un punto de entrada a un sistema.

**¿Cómo se soluciona?**  
Deshabilitar servicios innecesarios, restringir puertos mediante firewalls y limitar qué interfaces pueden aceptar conexiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría buscar listeners expuestos para identificar servicios vulnerables o utilizar uno comprometido para mantener comunicaciones.


## Bind

**¿Qué es?**  
Operación mediante la cual un proceso asocia un socket con una dirección IP y un puerto local para poder recibir o gestionar comunicaciones.

**¿Dónde lo encuentro?**  
En aplicaciones y servicios de red que necesitan abrir puertos para aceptar conexiones.

**¿Por qué me afecta?**  
Un servicio asociado a una dirección o interfaz incorrecta puede quedar expuesto a redes que no deberían acceder a él.

**¿Cómo se soluciona?**  
Configurar los servicios para escuchar únicamente en las interfaces y puertos necesarios y restringir el acceso mediante controles de red.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar un servicio que esté escuchando en una interfaz demasiado expuesta para intentar acceder al sistema.


## Network Interface

**¿Qué es?**  
Componente lógico mediante el cual un sistema se conecta y comunica con una red, utilizando parámetros como dirección IP y configuración de enlace.

**¿Dónde lo encuentro?**  
En computadoras, servidores, máquinas virtuales, dispositivos de red y sistemas cloud.

**¿Por qué me afecta?**  
Las interfaces determinan cómo un sistema se conecta a diferentes redes y pueden influir directamente en su exposición.

**¿Cómo se soluciona?**  
Configurar correctamente las interfaces, limitar redes innecesarias y aplicar controles de acceso y segmentación.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría identificar interfaces accesibles para descubrir redes conectadas al sistema y ampliar sus posibilidades de movimiento.


## NIC

**¿Qué es?**  
Network Interface Card es el componente de hardware o adaptador que permite a un dispositivo conectarse a una red.

**¿Dónde lo encuentro?**  
En computadoras, servidores, estaciones de trabajo, dispositivos de red y sistemas con conectividad Ethernet o inalámbrica.

**¿Por qué me afecta?**  
Una NIC proporciona la conectividad física o inalámbrica necesaria para las comunicaciones y puede representar una vía de acceso a la red.

**¿Cómo se soluciona?**  
Mantener sus controladores actualizados, configurar correctamente la conectividad y aplicar controles de acceso y seguridad de red.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar aprovechar una conexión de red comprometida o una configuración insegura asociada con la NIC para acceder a recursos de la red.
