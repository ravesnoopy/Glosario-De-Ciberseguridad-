
## Initial Access

**¿Qué es?**  
Initial Access es una táctica de MITRE ATT&CK que representa las técnicas utilizadas por los atacantes para obtener una primera entrada a un sistema o red.

**¿Dónde lo encuentro?**  
En correos de phishing, aplicaciones públicas, servicios remotos, cuentas comprometidas y otros puntos de entrada expuestos.

**¿Por qué me afecta?**  
Un acceso inicial exitoso permite al atacante establecer una posición desde la cual puede desarrollar otras etapas del ataque.

**¿Cómo se soluciona?**  
Reduciendo la superficie de ataque, protegiendo credenciales, aplicando MFA, actualizando sistemas y capacitando a los usuarios frente a técnicas de ingeniería social.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar phishing, credenciales válidas o explotar una aplicación expuesta para conseguir acceso inicial a la infraestructura.

## Execution

**¿Qué es?**  
Execution es una táctica de MITRE ATT&CK que agrupa técnicas utilizadas para ejecutar código o comandos controlados por el atacante.

**¿Dónde lo encuentro?**  
En sistemas operativos, scripts, intérpretes de comandos, aplicaciones, servicios y herramientas administrativas.

**¿Por qué me afecta?**  
La ejecución de código malicioso permite al atacante realizar acciones dentro del sistema después de obtener acceso.

**¿Cómo se soluciona?**  
Restringiendo la ejecución de software y scripts, aplicando mínimo privilegio, utilizando controles de endpoint y monitoreando procesos y comandos sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede ejecutar comandos, scripts o malware para continuar el ataque y realizar acciones sobre el sistema comprometido.

## Persistence

**¿Qué es?**  
Persistence es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para mantener el acceso a un sistema después de obtener una posición inicial.

**¿Dónde lo encuentro?**  
En cuentas, servicios, tareas programadas, mecanismos de inicio automático, aplicaciones y configuraciones del sistema.

**¿Por qué me afecta?**  
La persistencia permite que un atacante conserve acceso incluso después de reinicios, cierres de sesión o intentos parciales de recuperación.

**¿Cómo se soluciona?**  
Revisando mecanismos de inicio y persistencia, eliminando cuentas innecesarias, monitoreando cambios del sistema y aplicando mínimo privilegio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede crear tareas programadas, modificar mecanismos de inicio o establecer cuentas adicionales para recuperar el acceso posteriormente.

## Privilege Escalation

**¿Qué es?**  
Privilege Escalation es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para obtener permisos superiores a los que inicialmente posee el atacante.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, cuentas, configuraciones y servicios con permisos excesivos o vulnerabilidades.

**¿Por qué me afecta?**  
Obtener privilegios elevados puede permitir al atacante acceder a información sensible, modificar configuraciones críticas o controlar otros recursos.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, corrigiendo vulnerabilidades, protegiendo cuentas administrativas y monitoreando cambios de privilegios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar una vulnerabilidad o una configuración incorrecta para pasar de una cuenta con pocos permisos a una cuenta con mayores privilegios.

## Defense Evasion

**¿Qué es?**  
Defense Evasion es una táctica de MITRE ATT&CK que agrupa técnicas utilizadas para evitar ser detectado o dificultar las acciones de los mecanismos de seguridad.

**¿Dónde lo encuentro?**  
En sistemas comprometidos, malware, procesos, archivos, configuraciones y herramientas utilizadas durante una intrusión.

**¿Por qué me afecta?**  
La evasión puede retrasar la detección y permitir que un atacante permanezca activo durante más tiempo dentro del entorno.

**¿Cómo se soluciona?**  
Centralizando registros, utilizando EDR y otras herramientas de detección, protegiendo controles de seguridad y monitoreando comportamientos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede eliminar o modificar evidencias, ocultar archivos, utilizar herramientas legítimas o desactivar mecanismos de seguridad para reducir la probabilidad de detección.

## Credential Access

**¿Qué es?**  
Credential Access es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para obtener credenciales, secretos o información utilizada para autenticarse.

**¿Dónde lo encuentro?**  
En sistemas operativos, navegadores, gestores de credenciales, memoria, bases de datos, archivos de configuración y servicios de autenticación.

**¿Por qué me afecta?**  
El robo de credenciales puede proporcionar acceso a cuentas, sistemas y recursos adicionales sin necesidad de explotar nuevas vulnerabilidades.

**¿Cómo se soluciona?**  
Utilizando MFA, protegiendo credenciales, aplicando mínimo privilegio, evitando su almacenamiento inseguro y monitoreando actividades relacionadas con su acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener contraseñas, tokens, claves o hashes para autenticarse como usuarios legítimos y ampliar su acceso.

## Discovery

**¿Qué es?**  
Discovery es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para recopilar información sobre el entorno comprometido.

**¿Dónde lo encuentro?**  
En sistemas, redes, directorios, servicios, cuentas, dispositivos y recursos cloud accesibles desde el entorno comprometido.

**¿Por qué me afecta?**  
La información obtenida durante el reconocimiento interno ayuda al atacante a identificar sistemas importantes, cuentas privilegiadas y posibles rutas de ataque.

**¿Cómo se soluciona?**  
Limitando privilegios, segmentando la red, controlando el acceso a información interna y monitoreando actividades de enumeración y reconocimiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar usuarios, equipos, recursos compartidos, servicios y relaciones de red para planificar sus siguientes movimientos.

## Lateral Movement

**¿Qué es?**  
Lateral Movement es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para desplazarse desde un sistema comprometido hacia otros sistemas dentro del entorno.

**¿Dónde lo encuentro?**  
En redes internas, dominios corporativos, servicios remotos, recursos compartidos y sistemas con relaciones de confianza.

**¿Por qué me afecta?**  
El movimiento lateral permite que un compromiso limitado se convierta en una intrusión más amplia dentro de la organización.

**¿Cómo se soluciona?**  
Aplicando segmentación de red, mínimo privilegio, MFA, controles de acceso y monitoreo de conexiones entre sistemas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas, servicios remotos o recursos compartidos para desplazarse desde un equipo comprometido hacia otros sistemas.

## Collection

**¿Qué es?**  
Collection es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para recopilar información de interés antes de otras acciones, como la exfiltración.

**¿Dónde lo encuentro?**  
En documentos, correos electrónicos, bases de datos, sistemas de archivos, dispositivos y otros repositorios de información.

**¿Por qué me afecta?**  
La recopilación de información permite al atacante identificar y preparar datos sensibles para su posterior uso, robo o destrucción.

**¿Cómo se soluciona?**  
Aplicando controles de acceso, clasificación de información, mínimo privilegio, monitoreo de acceso a datos y protección de repositorios sensibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar documentos, correos, bases de datos u otros archivos relevantes y reunirlos en ubicaciones controladas por el atacante.

## Command and Control

**¿Qué es?**  
Command and Control es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para establecer comunicación entre sistemas comprometidos y la infraestructura controlada por el atacante.

**¿Dónde lo encuentro?**  
En conexiones de red salientes, servidores comprometidos, dominios maliciosos, DNS, HTTP/HTTPS y otros canales de comunicación.

**¿Por qué me afecta?**  
Un canal de Command and Control permite al atacante enviar instrucciones, recibir información y mantener control sobre sistemas comprometidos.

**¿Cómo se soluciona?**  
Filtrando tráfico de red, monitoreando conexiones salientes, utilizando DNS seguro y controles de endpoint, y bloqueando infraestructura maliciosa conocida.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede establecer comunicaciones periódicas con servidores bajo su control para enviar comandos, recibir instrucciones o transferir información.

## Exfiltration

**¿Qué es?**  
Exfiltration es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para transferir datos desde un entorno comprometido hacia una ubicación controlada por el atacante.

**¿Dónde lo encuentro?**  
En tráfico de red saliente, servicios cloud, canales de comunicación, servidores externos y sistemas comprometidos que contienen información sensible.

**¿Por qué me afecta?**  
La exfiltración puede provocar la pérdida de información confidencial, propiedad intelectual, datos personales o información empresarial.

**¿Cómo se soluciona?**  
Aplicando controles de salida, DLP cuando corresponda, segmentación, mínimo privilegio y monitoreo de transferencias de datos inusuales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprimir, dividir o transferir información recopilada hacia infraestructura externa bajo su control.

## Impact

**¿Qué es?**  
Impact es una táctica de MITRE ATT&CK que comprende técnicas utilizadas para manipular, interrumpir, destruir o afectar negativamente sistemas y recursos.

**¿Dónde lo encuentro?**  
En sistemas de producción, servidores, bases de datos, dispositivos, infraestructura cloud y otros recursos críticos.

**¿Por qué me afecta?**  
Las acciones de impacto pueden interrumpir operaciones, destruir información, cifrar sistemas o generar pérdidas económicas y operativas.

**¿Cómo se soluciona?**  
Manteniendo respaldos seguros, aplicando segmentación, controles de acceso, planes de recuperación y monitoreo de actividades destructivas o anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cifrar o destruir datos, interrumpir servicios o manipular sistemas para provocar daños operativos o económicos.
