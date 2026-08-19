
## Process Name

**¿Qué es?**  
Process Name es el nombre asociado a un proceso que está ejecutándose en un sistema operativo.

**¿Dónde lo encuentro?**  
En administradores de tareas, EDR, logs del sistema, herramientas de monitoreo y registros de procesos.

**¿Por qué me afecta?**  
Permite identificar qué programa está ejecutándose y detectar procesos inesperados o asociados con actividad maliciosa.

**¿Cómo se soluciona?**  
Monitoreando procesos, verificando su ubicación y firma, y estableciendo detecciones para procesos sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede ejecutar malware con nombres similares a procesos legítimos para dificultar su identificación.

## Process ID

**¿Qué es?**  
Process ID (PID) es un identificador numérico asignado por el sistema operativo a un proceso durante su ejecución.

**¿Dónde lo encuentro?**  
En administradores de tareas, comandos del sistema, EDR, herramientas forenses y registros de procesos.

**¿Por qué me afecta?**  
Permite relacionar procesos con conexiones, archivos, usuarios y otros eventos durante una investigación.

**¿Cómo se soluciona?**  
Registrando y correlacionando los PID con otros eventos de telemetría disponibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar procesos legítimos y sus PID para ejecutar código malicioso dentro de procesos existentes o realizar Process Injection.

## Parent Process ID

**¿Qué es?**  
Parent Process ID (PPID) es el identificador del proceso que creó o inició otro proceso.

**¿Dónde lo encuentro?**  
En EDR, logs de procesos, herramientas de administración y sistemas de monitoreo de endpoints.

**¿Por qué me afecta?**  
La relación entre procesos puede revelar comportamientos anómalos, como un proceso de Office iniciando una shell o un proceso del sistema ejecutando contenido inesperado.

**¿Cómo se soluciona?**  
Monitoreando las relaciones padre-hijo y creando detecciones para cadenas de procesos inusuales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar procesos legítimos como padres para ejecutar código malicioso y mezclarse con la actividad normal del sistema.

## Command Line

**¿Qué es?**  
Command Line es la cadena de argumentos e instrucciones utilizada para iniciar o controlar un proceso.

**¿Dónde lo encuentro?**  
En EDR, logs de procesos, Windows Event Logs, herramientas de administración y sistemas de monitoreo.

**¿Por qué me afecta?**  
Puede revelar comandos, parámetros, rutas y acciones ejecutadas, proporcionando evidencia importante durante una investigación.

**¿Cómo se soluciona?**  
Registrando líneas de comandos, protegiendo los logs y creando detecciones para patrones sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar comandos maliciosos, scripts o parámetros de herramientas legítimas para ejecutar acciones sin necesidad de instalar herramientas adicionales.

## File Path

**¿Qué es?**  
File Path es la ubicación donde se encuentra un archivo dentro de un sistema de archivos.

**¿Dónde lo encuentro?**  
En logs de procesos, EDR, sistemas operativos, herramientas forenses y registros de archivos.

**¿Por qué me afecta?**  
La ubicación de un archivo puede ayudar a determinar si un ejecutable pertenece a una instalación legítima o si se encuentra en una ubicación sospechosa.

**¿Cómo se soluciona?**  
Monitoreando rutas sensibles, verificando permisos y analizando archivos ejecutables ubicados en directorios inesperados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede colocar malware en directorios accesibles o utilizar rutas que imiten ubicaciones legítimas para dificultar su detección.

## File Hash

**¿Qué es?**  
File Hash es un valor calculado a partir del contenido de un archivo que permite identificar una versión específica del mismo.

**¿Dónde lo encuentro?**  
En EDR, antivirus, sistemas de análisis de malware, threat intelligence y herramientas forenses.

**¿Por qué me afecta?**  
Permite comparar archivos con muestras conocidas y utilizar hashes como indicadores durante una investigación.

**¿Cómo se soluciona?**  
Comparando hashes con fuentes confiables y combinándolos con análisis de comportamiento y otros indicadores.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar un archivo malicioso para generar un hash diferente y evitar detecciones basadas únicamente en ese valor.

## User Agent

**¿Qué es?**  
User Agent es una cadena de identificación enviada por un cliente HTTP para indicar información sobre el software que realiza una solicitud.

**¿Dónde lo encuentro?**  
En logs de servidores web, proxies, firewalls, aplicaciones y herramientas de análisis de tráfico HTTP.

**¿Por qué me afecta?**  
Puede ayudar a identificar clientes y detectar patrones de comunicación anómalos o herramientas utilizadas durante un ataque.

**¿Cómo se soluciona?**  
Monitoreando User Agents inusuales, correlacionándolos con otros datos y evitando confiar únicamente en este campo para autenticar clientes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar el User Agent para imitar navegadores legítimos y dificultar la identificación de tráfico automatizado o malicioso.

## DNS Query

**¿Qué es?**  
DNS Query es una solicitud realizada para obtener información asociada con un nombre de dominio, como su dirección IP u otros registros DNS.

**¿Dónde lo encuentro?**  
En servidores DNS, resolvers, firewalls, sistemas EDR, SIEM y capturas de tráfico de red.

**¿Por qué me afecta?**  
Las consultas DNS pueden revelar dominios maliciosos, patrones de reconocimiento, conexiones C2 o intentos de exfiltración mediante DNS.

**¿Cómo se soluciona?**  
Monitoreando consultas DNS, filtrando dominios maliciosos y detectando patrones anómalos como dominios generados automáticamente o consultas de alta frecuencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar consultas DNS para localizar infraestructura C2, realizar reconocimiento o transportar información mediante DNS tunneling.
