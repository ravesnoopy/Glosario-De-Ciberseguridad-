
## DNS

**¿Qué es?**  
Sistema que traduce nombres de dominio a direcciones IP y permite localizar servicios dentro de una red.

**¿Dónde lo encuentro?**  
En redes corporativas, Internet, servidores, dispositivos y aplicaciones que necesitan resolver nombres de dominio.

**¿Por qué me afecta?**  
DNS puede revelar comunicaciones, facilitar ataques de red o ser utilizado para resolver infraestructura maliciosa.

**¿Cómo se soluciona?**  
Utilizar servidores DNS confiables, monitorear consultas, restringir resoluciones innecesarias y aplicar controles contra dominios maliciosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar DNS para localizar infraestructura maliciosa, realizar reconocimiento o establecer comunicaciones con sistemas comprometidos.


## DHCP

**¿Qué es?**  
Protocolo que asigna automáticamente parámetros de configuración de red, como direcciones IP, puerta de enlace y servidores DNS.

**¿Dónde lo encuentro?**  
En redes domésticas, empresariales y otros entornos donde los dispositivos reciben configuración de red automáticamente.

**¿Por qué me afecta?**  
Un servidor DHCP no autorizado puede proporcionar configuraciones maliciosas y redirigir el tráfico de los dispositivos afectados.

**¿Cómo se soluciona?**  
Utilizar DHCP Snooping cuando esté disponible, controlar los dispositivos autorizados y monitorear servidores DHCP no reconocidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría introducir un servidor DHCP no autorizado para proporcionar una configuración de red controlada por él.


## HTTP

**¿Qué es?**  
Protocolo utilizado para transferir recursos y solicitudes entre clientes y servidores web.

**¿Dónde lo encuentro?**  
En sitios web, APIs, aplicaciones web, navegadores y servicios que utilizan comunicación HTTP.

**¿Por qué me afecta?**  
HTTP no proporciona cifrado de transporte por sí mismo, por lo que la información transmitida puede quedar expuesta o ser manipulada.

**¿Cómo se soluciona?**  
Utilizar HTTPS, configurar correctamente los servidores web y proteger las aplicaciones contra vulnerabilidades web.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría interceptar o manipular comunicaciones HTTP cuando no estén protegidas por mecanismos de cifrado.


## HTTPS

**¿Qué es?**  
Versión de HTTP protegida mediante TLS que proporciona cifrado, autenticación del servidor e integridad de las comunicaciones.

**¿Dónde lo encuentro?**  
En sitios web, APIs, aplicaciones web y servicios que transmiten información mediante conexiones seguras.

**¿Por qué me afecta?**  
Protege los datos durante el tránsito y reduce el riesgo de interceptación o modificación de las comunicaciones.

**¿Cómo se soluciona?**  
Utilizar configuraciones TLS seguras, certificados válidos y versiones criptográficas actualizadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría aprovechar certificados inválidos, configuraciones débiles o engañar al usuario para establecer comunicación con un sitio controlado por el atacante.


## FTP

**¿Qué es?**  
File Transfer Protocol es un protocolo utilizado para transferir archivos entre clientes y servidores.

**¿Dónde lo encuentro?**  
En servidores de transferencia de archivos, sistemas heredados y entornos donde se requiere intercambio de archivos mediante FTP.

**¿Por qué me afecta?**  
FTP tradicionalmente transmite credenciales y datos sin cifrado, lo que puede permitir su exposición durante el tránsito.

**¿Cómo se soluciona?**  
Evitar FTP cuando sea posible y utilizar alternativas seguras como SFTP o mecanismos de transferencia protegidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría interceptar credenciales o archivos transmitidos mediante una conexión FTP sin protección.


## SFTP

**¿Qué es?**  
SSH File Transfer Protocol es un protocolo para transferir y administrar archivos de forma segura mediante una conexión SSH.

**¿Dónde lo encuentro?**  
En servidores Linux, sistemas de transferencia de archivos, automatizaciones y entornos empresariales que requieren intercambio seguro de información.

**¿Por qué me afecta?**  
Protege las credenciales y los datos durante la transferencia, pero una cuenta comprometida puede proporcionar acceso a los archivos disponibles.

**¿Cómo se soluciona?**  
Utilizar autenticación robusta, mínimo privilegio, restricciones de acceso y monitoreo de las sesiones SFTP.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar credenciales comprometidas para acceder a un servidor SFTP y consultar, modificar o extraer archivos autorizados para esa cuenta.


## SSH

**¿Qué es?**  
Secure Shell es un protocolo que permite administrar sistemas y ejecutar comandos de forma remota mediante una conexión cifrada.

**¿Dónde lo encuentro?**  
Principalmente en servidores Linux y Unix, dispositivos de red, sistemas cloud y entornos de administración remota.

**¿Por qué me afecta?**  
Una cuenta SSH comprometida puede proporcionar acceso remoto al sistema y permitir acciones dependiendo de sus privilegios.

**¿Cómo se soluciona?**  
Utilizar autenticación mediante claves cuando corresponda, restringir accesos, aplicar mínimo privilegio, mantener el servicio actualizado y monitorear sesiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar credenciales o claves comprometidas para acceder remotamente a sistemas y realizar acciones con los permisos obtenidos.


## Telnet

**¿Qué es?**  
Protocolo utilizado para establecer sesiones remotas de administración mediante una conexión que tradicionalmente no cifra las comunicaciones.

**¿Dónde lo encuentro?**  
Principalmente en sistemas heredados, dispositivos antiguos y entornos donde todavía existen servicios Telnet habilitados.

**¿Por qué me afecta?**  
La ausencia de cifrado puede exponer credenciales y datos transmitidos durante una sesión.

**¿Cómo se soluciona?**  
Deshabilitar Telnet cuando no sea necesario y sustituirlo por protocolos seguros como SSH.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría interceptar las comunicaciones de una sesión Telnet para obtener credenciales o información transmitida.
