
## Initial Access

**¿Qué es?**  
Initial Access es una táctica de MITRE ATT&CK que representa las técnicas utilizadas por un adversario para obtener acceso inicial a un sistema o entorno.

**¿Dónde lo encuentro?**  
En aplicaciones expuestas, servicios remotos, cuentas comprometidas, correos electrónicos, dispositivos y otros puntos de entrada.

**¿Por qué me afecta?**  
Un acceso inicial exitoso puede proporcionar al atacante el punto de entrada necesario para comenzar otras actividades dentro del entorno.

**¿Cómo se soluciona?**  
Aplicando MFA, gestión de vulnerabilidades, controles de acceso, filtrado de correo, hardening y monitoreo de servicios expuestos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar phishing, explotación de aplicaciones públicas, credenciales válidas o servicios remotos para obtener acceso al entorno.

## Persistence

**¿Qué es?**  
Persistence es una táctica de MITRE ATT&CK que representa las técnicas utilizadas por un adversario para mantener acceso a un sistema o entorno después de reinicios, cambios de credenciales u otras interrupciones.

**¿Dónde lo encuentro?**  
En cuentas, servicios, tareas programadas, mecanismos de inicio automático, aplicaciones y configuraciones del sistema.

**¿Por qué me afecta?**  
La persistencia permite que un atacante conserve acceso incluso después de que algunas partes del ataque hayan sido detectadas o interrumpidas.

**¿Cómo se soluciona?**  
Revisando mecanismos de persistencia, controlando cuentas y servicios, monitoreando cambios y eliminando los mecanismos no autorizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede crear cuentas, tareas programadas, servicios o modificar configuraciones para recuperar acceso posteriormente.

## Execution

**¿Qué es?**  
Execution es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para ejecutar código o comandos controlados por un adversario.

**¿Dónde lo encuentro?**  
En procesos, intérpretes de comandos, scripts, aplicaciones, servicios y herramientas administrativas de los sistemas.

**¿Por qué me afecta?**  
La ejecución permite que un atacante convierta el acceso obtenido en acciones concretas dentro del sistema.

**¿Cómo se soluciona?**  
Aplicando controles de ejecución, restricciones de scripts, mínimo privilegio, allowlisting cuando sea apropiado y monitoreo de procesos y comandos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede ejecutar malware, scripts o comandos mediante herramientas legítimas del sistema para realizar acciones maliciosas.

## Privilege Escalation

**¿Qué es?**  
Privilege Escalation es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para obtener permisos superiores a los inicialmente disponibles.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, servicios, cuentas y configuraciones que contienen permisos o vulnerabilidades explotables.

**¿Por qué me afecta?**  
Un atacante con mayores privilegios puede acceder a más recursos, modificar sistemas y realizar acciones administrativas.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, corrigiendo vulnerabilidades, separando cuentas administrativas y monitoreando cambios de privilegios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar vulnerabilidades, configuraciones débiles o credenciales privilegiadas para obtener permisos superiores.

## Defense Evasion

**¿Qué es?**  
Defense Evasion es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para evitar ser detectado o interferir con los mecanismos de seguridad.

**¿Dónde lo encuentro?**  
En endpoints, sistemas de archivos, registros, procesos, herramientas de seguridad y configuraciones del sistema.

**¿Por qué me afecta?**  
Permite que un atacante continúe sus actividades durante más tiempo sin generar alertas o evidencias claras.

**¿Cómo se soluciona?**  
Centralizando registros, protegiendo herramientas de seguridad, monitoreando comportamientos sospechosos y utilizando múltiples capas de detección.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede deshabilitar controles, eliminar registros, modificar archivos o utilizar herramientas legítimas para ocultar sus acciones.

## Credential Access

**¿Qué es?**  
Credential Access es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para robar o adquirir credenciales y otros secretos de autenticación.

**¿Dónde lo encuentro?**  
En sistemas operativos, navegadores, gestores de credenciales, bases de datos, memoria, archivos y servicios de autenticación.

**¿Por qué me afecta?**  
Las credenciales comprometidas pueden permitir al atacante acceder a sistemas adicionales y hacerse pasar por usuarios legítimos.

**¿Cómo se soluciona?**  
Utilizando MFA, protección de credenciales, mínimo privilegio, rotación de credenciales y monitoreo de accesos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar phishing, credential dumping, keylogging u otras técnicas para obtener credenciales y reutilizarlas.

## Discovery

**¿Qué es?**  
Discovery es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para recopilar información sobre sistemas, usuarios, redes y recursos del entorno.

**¿Dónde lo encuentro?**  
En endpoints, redes, servicios de directorio, sistemas cloud y registros donde se puedan observar actividades de reconocimiento interno.

**¿Por qué me afecta?**  
El descubrimiento permite al atacante comprender el entorno y seleccionar objetivos de mayor valor.

**¿Cómo se soluciona?**  
Limitando permisos, segmentando redes, monitoreando actividades de reconocimiento y detectando consultas o comportamientos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar usuarios, equipos, recursos compartidos, servicios y relaciones de confianza para planificar sus siguientes movimientos.

## Lateral Movement

**¿Qué es?**  
Lateral Movement es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para desplazarse desde un sistema comprometido hacia otros sistemas dentro del entorno.

**¿Dónde lo encuentro?**  
En redes internas, Active Directory, servicios remotos, servidores, endpoints y sistemas con relaciones de confianza.

**¿Por qué me afecta?**  
Permite que un compromiso inicial se extienda hacia otros sistemas y aumente el alcance del incidente.

**¿Cómo se soluciona?**  
Utilizando segmentación de red, mínimo privilegio, MFA, controles sobre servicios remotos y monitoreo de autenticaciones internas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede reutilizar credenciales, utilizar servicios remotos o aprovechar relaciones de confianza para acceder a otros sistemas.

## Collection

**¿Qué es?**  
Collection es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para recopilar datos relevantes antes de utilizarlos o exfiltrarlos.

**¿Dónde lo encuentro?**  
En endpoints, servidores, bases de datos, recursos compartidos, buzones de correo y otros repositorios de información.

**¿Por qué me afecta?**  
La recopilación permite al atacante identificar y reunir información de valor para sus objetivos.

**¿Cómo se soluciona?**  
Aplicando controles de acceso, clasificación de datos, monitoreo de accesos y detección de actividades inusuales sobre información sensible.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar documentos, correos, bases de datos, credenciales u otros datos de interés y reunirlos antes de extraerlos.

## C2

**¿Qué es?**  
C2 (Command and Control) es la comunicación utilizada por un atacante para controlar sistemas comprometidos y enviar o recibir instrucciones.

**¿Dónde lo encuentro?**  
En tráfico de red, DNS, HTTP/HTTPS, conexiones a Internet, proxies, servidores remotos y otros canales de comunicación.

**¿Por qué me afecta?**  
Un canal C2 activo puede permitir que un atacante controle sistemas comprometidos y continúe ejecutando acciones remotamente.

**¿Cómo se soluciona?**  
Monitoreando tráfico de red, utilizando filtrado de DNS y firewall, analizando conexiones anómalas y detectando patrones de comunicación sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede establecer comunicaciones periódicas con infraestructura bajo su control para enviar comandos, recibir información o mantener acceso.

## Exfiltration

**¿Qué es?**  
Exfiltration es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para extraer datos desde un entorno comprometido hacia una ubicación controlada por el adversario.

**¿Dónde lo encuentro?**  
En tráfico de red, servicios cloud, servidores externos, canales de comunicación y sistemas donde se transfieren datos fuera de la organización.

**¿Por qué me afecta?**  
La exfiltración puede provocar pérdida de información confidencial, propiedad intelectual, datos personales o información estratégica.

**¿Cómo se soluciona?**  
Aplicando controles de salida, DLP, monitoreo de tráfico, clasificación de datos y detección de transferencias inusuales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprimir, cifrar y transferir información mediante canales legítimos o infraestructura controlada para evitar la detección.

## Impact

**¿Qué es?**  
Impact es una táctica de MITRE ATT&CK que representa las técnicas utilizadas para manipular, interrumpir, degradar o destruir sistemas y recursos.

**¿Dónde lo encuentro?**  
En sistemas críticos, servidores, bases de datos, infraestructura de red y servicios utilizados por una organización.

**¿Por qué me afecta?**  
Las acciones de impacto pueden interrumpir operaciones, destruir información, causar pérdidas económicas o afectar la disponibilidad de servicios.

**¿Cómo se soluciona?**  
Implementando respaldos, redundancia, recuperación ante desastres, segmentación, controles de acceso y monitoreo de actividades destructivas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cifrar datos mediante ransomware, destruir información, interrumpir servicios o manipular sistemas para afectar las operaciones.
