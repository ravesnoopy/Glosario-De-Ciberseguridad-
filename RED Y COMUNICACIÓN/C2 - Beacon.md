
## C2

**¿Qué es?**  
C2 (Command and Control) es la infraestructura o canal de comunicación que permite a un atacante controlar sistemas comprometidos y enviar o recibir instrucciones.

**¿Dónde lo encuentro?**  
En tráfico de red, DNS, HTTP/HTTPS, conexiones externas, proxies, servidores remotos y registros de comunicación de endpoints.

**¿Por qué me afecta?**  
Un canal C2 activo puede permitir que un atacante mantenga control remoto sobre sistemas comprometidos y continúe ejecutando acciones.

**¿Cómo se soluciona?**  
Monitoreando tráfico de red, filtrando conexiones de salida, analizando DNS y detectando patrones de comunicación anómalos o periódicos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede establecer un canal C2 para enviar comandos, recibir información, mantener acceso y controlar sistemas comprometidos.

## Beacon

**¿Qué es?**  
Beacon es un mecanismo mediante el cual un sistema comprometido se comunica periódicamente con una infraestructura C2 para indicar que está activo y, según el caso, recibir instrucciones.

**¿Dónde lo encuentro?**  
En tráfico de red, conexiones DNS, HTTP/HTTPS y otros protocolos utilizados por malware o herramientas de administración remota.

**¿Por qué me afecta?**  
Los beacons pueden proporcionar persistencia y comunicación con infraestructura externa, y sus patrones periódicos pueden ser una señal útil para detectar compromisos.

**¿Cómo se soluciona?**  
Analizando frecuencia, destinos, intervalos y características de las conexiones, y correlacionándolos con procesos y actividad de los endpoints.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar comunicaciones periódicas con su infraestructura C2 para mantener el control del sistema y recibir nuevas instrucciones sin generar conexiones constantes.
