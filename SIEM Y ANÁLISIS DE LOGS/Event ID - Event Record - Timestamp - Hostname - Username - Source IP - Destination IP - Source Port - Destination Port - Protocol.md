
## Event ID

**¿Qué es?**  
Event ID es un identificador numérico utilizado para distinguir un tipo específico de evento registrado por un sistema o aplicación.

**¿Dónde lo encuentro?**  
En logs de sistemas operativos, aplicaciones, servicios de red, SIEM y plataformas de monitoreo.

**¿Por qué me afecta?**  
Permite identificar rápidamente qué tipo de actividad ocurrió y facilita la correlación de eventos durante una investigación.

**¿Cómo se soluciona?**  
Configurando correctamente el registro de eventos, centralizando los logs y utilizando reglas de detección basadas en Event ID cuando sean relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar generar actividad que se mezcle con eventos legítimos o modificar configuraciones de logging para reducir la evidencia disponible.

## Event Record

**¿Qué es?**  
Event Record es el registro que contiene la información asociada con un evento ocurrido en un sistema, aplicación o dispositivo.

**¿Dónde lo encuentro?**  
En archivos de logs, Windows Event Log, servidores, aplicaciones, dispositivos de red y plataformas SIEM.

**¿Por qué me afecta?**  
Puede proporcionar evidencia sobre autenticaciones, procesos, conexiones, cambios de configuración y otras actividades relevantes para una investigación.

**¿Cómo se soluciona?**  
Centralizando los registros, protegiéndolos contra modificaciones y estableciendo políticas adecuadas de retención y monitoreo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar, alterar o evitar la generación de registros para dificultar la reconstrucción de sus actividades.

## Timestamp

**¿Qué es?**  
Timestamp es la fecha y hora asociada con un evento registrado, utilizada para establecer cuándo ocurrió una actividad.

**¿Dónde lo encuentro?**  
En logs de sistemas, aplicaciones, dispositivos de red, SIEM, EDR y herramientas de análisis forense.

**¿Por qué me afecta?**  
Permite construir una línea temporal y determinar la secuencia de eventos durante una investigación de seguridad.

**¿Cómo se soluciona?**  
Sincronizando los sistemas mediante fuentes de tiempo confiables y manteniendo configuraciones horarias consistentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar la hora del sistema o realizar acciones en momentos que dificulten su correlación con otros eventos.

## Hostname

**¿Qué es?**  
Hostname es el nombre asignado a un dispositivo dentro de una red para facilitar su identificación.

**¿Dónde lo encuentro?**  
En sistemas operativos, DNS, DHCP, logs, EDR, SIEM y herramientas de administración de infraestructura.

**¿Por qué me afecta?**  
Permite identificar qué equipo generó o recibió una actividad y relacionarla con otros eventos durante una investigación.

**¿Cómo se soluciona?**  
Manteniendo nombres consistentes, inventarios actualizados y correlacionando el hostname con otros identificadores del dispositivo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede recopilar hostnames durante el reconocimiento para identificar servidores, estaciones de trabajo y otros recursos de interés.

## Username

**¿Qué es?**  
Username es el identificador utilizado para asociar una cuenta con una persona, servicio o proceso dentro de un sistema.

**¿Dónde lo encuentro?**  
En logs de autenticación, sistemas operativos, aplicaciones, Active Directory, EDR y plataformas SIEM.

**¿Por qué me afecta?**  
Permite determinar qué cuenta realizó una acción y detectar actividades sospechosas relacionadas con credenciales.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, autenticación fuerte, monitoreo de cuentas y revisión de actividades asociadas con usuarios privilegiados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para autenticarse como un usuario legítimo y realizar acciones sin levantar sospechas inmediatas.

## Source IP

**¿Qué es?**  
Source IP es la dirección IP asociada al origen de una comunicación de red.

**¿Dónde lo encuentro?**  
En firewalls, routers, servidores, EDR, sistemas de detección y registros de conexiones.

**¿Por qué me afecta?**  
Permite identificar desde dónde se originó una conexión y ayuda a investigar reconocimiento, accesos no autorizados y comunicaciones sospechosas.

**¿Cómo se soluciona?**  
Monitoreando las conexiones, aplicando reglas de red y correlacionando la IP con otros datos disponibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar infraestructura intermedia, proxies o sistemas comprometidos para ocultar el origen real de sus conexiones.

## Destination IP

**¿Qué es?**  
Destination IP es la dirección IP del sistema o servicio al que se dirige una comunicación de red.

**¿Dónde lo encuentro?**  
En firewalls, routers, servidores, EDR, tráfico de red y registros de conexiones.

**¿Por qué me afecta?**  
Ayuda a identificar qué sistemas internos o externos están siendo contactados y puede revelar conexiones hacia infraestructura maliciosa.

**¿Cómo se soluciona?**  
Monitoreando destinos, aplicando filtrado de red y correlacionando las conexiones con inteligencia de amenazas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede establecer conexiones hacia una Destination IP controlada por él para recibir comandos, enviar información o descargar componentes.

## Source Port

**¿Qué es?**  
Source Port es el número de puerto utilizado por el sistema que inicia una comunicación para identificar el proceso o conexión correspondiente.

**¿Dónde lo encuentro?**  
En capturas de tráfico, firewalls, sistemas de detección y registros de conexiones TCP o UDP.

**¿Por qué me afecta?**  
Ayuda a distinguir conexiones individuales y puede proporcionar contexto sobre el comportamiento de una comunicación.

**¿Cómo se soluciona?**  
Monitoreando patrones de conexiones y correlacionando el puerto con el proceso, host y destino involucrados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar puertos de origen variables o efímeros para establecer múltiples conexiones y dificultar análisis basados únicamente en puertos.

## Destination Port

**¿Qué es?**  
Destination Port es el número de puerto asociado al servicio o proceso al que está dirigida una comunicación.

**¿Dónde lo encuentro?**  
En firewalls, servidores, escáneres de red, capturas PCAP y logs de conexiones.

**¿Por qué me afecta?**  
Permite identificar qué servicio está siendo contactado y detectar accesos a puertos inesperados o no autorizados.

**¿Cómo se soluciona?**  
Cerrando servicios innecesarios, restringiendo puertos mediante firewalls y monitoreando conexiones hacia servicios sensibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede escanear Destination Ports para identificar servicios disponibles y buscar aquellos que puedan ser vulnerables.

## Protocol

**¿Qué es?**  
Protocol es el conjunto de reglas que define cómo se estructuran, transmiten e interpretan los datos durante una comunicación entre sistemas.

**¿Dónde lo encuentro?**  
En redes, aplicaciones, sistemas operativos, dispositivos de infraestructura y registros de tráfico.

**¿Por qué me afecta?**  
Conocer el protocolo utilizado ayuda a comprender una comunicación y detectar comportamientos anómalos o protocolos inesperados.

**¿Cómo se soluciona?**  
Restringiendo protocolos innecesarios, utilizando versiones seguras y monitoreando comunicaciones que no correspondan al comportamiento esperado.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar protocolos legítimos para ocultar comunicaciones maliciosas, establecer C2 o transportar información dentro de tráfico aparentemente normal.
