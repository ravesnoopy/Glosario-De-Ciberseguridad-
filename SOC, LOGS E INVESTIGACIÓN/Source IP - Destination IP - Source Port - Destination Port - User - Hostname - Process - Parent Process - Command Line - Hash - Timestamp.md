
## Source IP

**¿Qué es?**  
Dirección IP del origen de una comunicación de red, es decir, del dispositivo o sistema que inicia o genera el tráfico.

**¿Dónde lo encuentro?**  
En logs de firewalls, servidores, routers, IDS/IPS, SIEM, aplicaciones y capturas de tráfico.

**¿Por qué me afecta?**  
Permite identificar el origen aparente de una conexión y correlacionarlo con otros eventos durante una investigación.

**¿Cómo se soluciona?**  
Validar la IP mediante múltiples fuentes y considerar NAT, proxies, VPN y otros mecanismos que pueden ocultar el origen real.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar una IP comprometida, proxy o infraestructura intermedia para dificultar la identificación de su origen real.


## Destination IP

**¿Qué es?**  
Dirección IP del destino al que se dirige una comunicación de red.

**¿Dónde lo encuentro?**  
En firewalls, routers, servidores, IDS/IPS, SIEM y capturas de tráfico.

**¿Por qué me afecta?**  
Permite determinar qué sistema o servicio recibió una comunicación y ayuda a identificar conexiones sospechosas.

**¿Cómo se soluciona?**  
Monitorear destinos relevantes y restringir comunicaciones innecesarias mediante segmentación y controles de red.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría dirigir conexiones hacia sistemas internos para realizar reconocimiento, movimiento lateral o hacia infraestructura externa para comunicarse con C2.


## Source Port

**¿Qué es?**  
Puerto utilizado por el origen de una comunicación para identificar el proceso o servicio asociado con el tráfico.

**¿Dónde lo encuentro?**  
En logs de red, firewalls, capturas de paquetes y herramientas de monitoreo.

**¿Por qué me afecta?**  
Ayuda a identificar patrones de comunicación y distinguir diferentes conexiones entre los mismos dispositivos.

**¿Cómo se soluciona?**  
Analizar puertos junto con IP, protocolo, proceso y contexto de la conexión.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar puertos de origen variables o patrones específicos para dificultar reglas de filtrado o análisis de tráfico.


## Destination Port

**¿Qué es?**  
Puerto utilizado por el destino para identificar el servicio o aplicación al que se dirige una comunicación.

**¿Dónde lo encuentro?**  
En firewalls, servidores, routers, IDS/IPS, capturas de red y SIEM.

**¿Por qué me afecta?**  
Permite determinar qué servicio está siendo contactado y ayuda a identificar accesos no autorizados o servicios expuestos.

**¿Cómo se soluciona?**  
Cerrar puertos innecesarios, restringir el acceso y monitorear conexiones hacia servicios críticos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría explorar puertos para identificar servicios disponibles y buscar vulnerabilidades asociadas.


## User

**¿Qué es?**  
Identidad asociada con una persona, cuenta de servicio o entidad que realiza acciones dentro de un sistema.

**¿Dónde lo encuentro?**  
En eventos de autenticación, Active Directory, aplicaciones, sistemas operativos, SIEM y registros de auditoría.

**¿Por qué me afecta?**  
Permite atribuir acciones a una identidad y detectar accesos anómalos, uso indebido de cuentas o credenciales comprometidas.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, MFA, controles de acceso y monitoreo de actividades de las cuentas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría comprometer una cuenta legítima y utilizar sus permisos para acceder a sistemas o realizar acciones sin levantar sospechas inmediatas.


## Hostname

**¿Qué es?**  
Nombre asignado a un dispositivo o sistema dentro de una red para identificarlo de forma más legible que mediante su dirección IP.

**¿Dónde lo encuentro?**  
En sistemas operativos, DNS, Active Directory, DHCP, logs, EDR y herramientas de administración.

**¿Por qué me afecta?**  
Facilita identificar sistemas involucrados en eventos y correlacionar actividad durante una investigación.

**¿Cómo se soluciona?**  
Mantener una convención de nombres consistente y asociar correctamente los hostnames con inventarios y activos conocidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría recopilar hostnames durante el reconocimiento para identificar servidores, estaciones de trabajo y otros recursos.


## Process

**¿Qué es?**  
Instancia en ejecución de un programa dentro de un sistema operativo, con recursos y contexto propios.

**¿Dónde lo encuentro?**  
En sistemas operativos, EDR, Sysmon, administradores de tareas y registros de eventos.

**¿Por qué me afecta?**  
Los procesos permiten identificar qué programas se ejecutaron y detectar ejecuciones inusuales o maliciosas.

**¿Cómo se soluciona?**  
Monitorear procesos relevantes, analizar su origen y relación con otros eventos y aplicar controles de ejecución.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría ejecutar malware o abusar de procesos legítimos para realizar acciones maliciosas.


## Parent Process

**¿Qué es?**  
Proceso que inició o creó otro proceso, estableciendo una relación padre-hijo dentro del sistema operativo.

**¿Dónde lo encuentro?**  
En EDR, Sysmon, logs de procesos y herramientas de análisis de endpoints.

**¿Por qué me afecta?**  
La relación entre procesos puede revelar cadenas de ejecución anómalas y proporcionar evidencia sobre cómo se inició una actividad.

**¿Cómo se soluciona?**  
Registrar relaciones padre-hijo y crear detecciones para combinaciones de procesos inusuales.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría abusar de procesos legítimos o técnicas de ejecución que hagan que una actividad maliciosa parezca originarse de un proceso esperado.


## Command Line

**¿Qué es?**  
Texto que contiene el programa ejecutado junto con los argumentos y parámetros utilizados durante su ejecución.

**¿Dónde lo encuentro?**  
En EDR, Sysmon, registros de Windows, herramientas de administración y sistemas SIEM.

**¿Por qué me afecta?**  
Puede revelar comandos, rutas, parámetros y acciones realizadas por un proceso, siendo una fuente importante de evidencia.

**¿Cómo se soluciona?**  
Registrar la línea de comandos, proteger los logs y crear detecciones sobre patrones de ejecución sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría ejecutar comandos maliciosos, utilizar parámetros para evadir controles o abusar de herramientas legítimas del sistema.


## Hash

**¿Qué es?**  
Valor calculado a partir de datos, como un archivo, que permite identificar su contenido de manera práctica y detectar cambios.

**¿Dónde lo encuentro?**  
En EDR, análisis de malware, sistemas de archivos, repositorios de inteligencia y registros de seguridad.

**¿Por qué me afecta?**  
Permite comparar archivos con indicadores conocidos y detectar archivos que coinciden con malware previamente identificado.

**¿Cómo se soluciona?**  
Calcular y comparar hashes mediante fuentes confiables, teniendo en cuenta que un hash por sí solo no demuestra que un archivo sea malicioso.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría modificar un archivo malicioso para producir un hash diferente y evitar detecciones basadas exclusivamente en hashes conocidos.


## Timestamp

**¿Qué es?**  
Marca temporal asociada con un evento que indica cuándo ocurrió una actividad o fue registrada por un sistema.

**¿Dónde lo encuentro?**  
En logs, eventos de seguridad, archivos, bases de datos, capturas de red y sistemas SIEM.

**¿Por qué me afecta?**  
Permite construir timelines, correlacionar eventos y determinar la secuencia temporal de un incidente.

**¿Cómo se soluciona?**  
Sincronizar relojes, conservar zonas horarias y validar las marcas de tiempo entre diferentes fuentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría alterar o eliminar registros y manipular marcas temporales para dificultar la reconstrucción de sus actividades.
