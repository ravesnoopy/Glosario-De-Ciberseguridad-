
## Web Shell

**¿Qué es?**  
Una Web Shell es un script o mecanismo malicioso instalado en un servidor web que permite al atacante ejecutar comandos o realizar acciones de forma remota.

**¿Dónde lo encuentro?**  
En servidores web comprometidos, normalmente dentro de directorios utilizados por aplicaciones web y que permiten la ejecución de scripts.

**¿Por qué me afecta?**  
Puede proporcionar acceso persistente al servidor y permitir la ejecución de comandos, manipulación de archivos o acceso a información sensible.

**¿Cómo se soluciona?**  
Eliminando archivos maliciosos, corrigiendo la vulnerabilidad que permitió su instalación, revisando cambios en archivos y restringiendo permisos de escritura y ejecución.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede instalar una Web Shell después de explotar una vulnerabilidad para ejecutar comandos y mantener acceso al servidor comprometido.

## Reverse Shell

**¿Qué es?**  
Una Reverse Shell es una conexión en la que el sistema comprometido inicia una comunicación hacia el sistema controlado por el atacante y proporciona una interfaz para ejecutar comandos.

**¿Dónde lo encuentro?**  
En sistemas comprometidos, servidores, estaciones de trabajo y durante actividades de explotación o pruebas de penetración.

**¿Por qué me afecta?**  
Puede proporcionar al atacante una interfaz interactiva para controlar un sistema comprometido y continuar con otras etapas del ataque.

**¿Cómo se soluciona?**  
Controlando conexiones salientes, aplicando segmentación de red, utilizando firewalls y monitoreando procesos y comunicaciones anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de conseguir ejecución de código, puede hacer que el sistema comprometido establezca una conexión hacia su infraestructura para obtener una sesión remota.

## Bind Shell

**¿Qué es?**  
Una Bind Shell es una interfaz de comandos que escucha en un puerto del sistema comprometido y permite que un tercero se conecte para ejecutar comandos.

**¿Dónde lo encuentro?**  
En sistemas comprometidos donde un proceso malicioso abre un puerto de escucha para aceptar conexiones remotas.

**¿Por qué me afecta?**  
Puede crear un punto de acceso remoto no autorizado y exponer un servicio adicional que facilite el control del sistema.

**¿Cómo se soluciona?**  
Bloqueando puertos innecesarios, restringiendo conexiones mediante firewalls, eliminando procesos maliciosos y monitoreando puertos y servicios inesperados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede iniciar una shell que escuche en un puerto y utilizarla para conectarse posteriormente al sistema comprometido y ejecutar comandos.

## C2

**¿Qué es?**  
C2 (Command and Control) es la infraestructura o mecanismo mediante el cual un atacante se comunica con sistemas comprometidos para enviar instrucciones y recibir información.

**¿Dónde lo encuentro?**  
En conexiones de red entre dispositivos comprometidos e infraestructura controlada por atacantes, utilizando canales como HTTP/HTTPS, DNS u otros protocolos.

**¿Por qué me afecta?**  
Un canal C2 permite mantener el control de sistemas comprometidos y coordinar actividades posteriores al acceso inicial.

**¿Cómo se soluciona?**  
Monitoreando tráfico de red, controlando conexiones salientes, bloqueando infraestructura maliciosa y utilizando herramientas de detección en endpoints y redes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede establecer un canal C2 para enviar comandos, recibir resultados, mantener acceso y coordinar acciones sobre los sistemas comprometidos.

## Beacon

**¿Qué es?**  
Un Beacon es un mecanismo de comunicación utilizado por malware o herramientas de post-explotación para contactar periódicamente con una infraestructura de Command and Control.

**¿Dónde lo encuentro?**  
En sistemas comprometidos que mantienen comunicación periódica con servidores o infraestructura controlada por un atacante.

**¿Por qué me afecta?**  
Los Beacons pueden mantener una conexión de control persistente y utilizar patrones de comunicación diseñados para mezclarse con tráfico aparentemente legítimo.

**¿Cómo se soluciona?**  
Analizando patrones de tráfico, frecuencia de conexiones, dominios, procesos asociados y comportamiento de red mediante herramientas de monitoreo y detección.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar un Beacon para comunicarse periódicamente con su infraestructura, recibir instrucciones y enviar información desde un sistema comprometido.
