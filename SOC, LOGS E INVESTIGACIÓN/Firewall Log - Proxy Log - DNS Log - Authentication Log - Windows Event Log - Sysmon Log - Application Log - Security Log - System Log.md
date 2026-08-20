
## Firewall Log

**¿Qué es?**  
Firewall Log es un registro de las conexiones y eventos de red procesados por un firewall, incluyendo tráfico permitido, bloqueado o rechazado.

**¿Dónde lo encuentro?**  
En firewalls de red, firewalls de host, plataformas cloud y SIEM que reciben sus registros.

**¿Por qué me afecta?**  
Permite identificar conexiones sospechosas, escaneos, intentos de acceso y comunicaciones con infraestructura potencialmente maliciosa.

**¿Cómo se soluciona?**  
Habilitando el registro de eventos relevantes, centralizándolo y creando reglas de monitoreo para tráfico anómalo o no autorizado.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar puertos o protocolos permitidos para intentar ocultar comunicaciones maliciosas dentro del tráfico autorizado.

## Proxy Log

**¿Qué es?**  
Proxy Log es un registro de las solicitudes realizadas a través de un servidor proxy, incluyendo información sobre clientes, destinos y recursos solicitados.

**¿Dónde lo encuentro?**  
En proxies web, gateways de Internet, sistemas de filtrado y plataformas SIEM.

**¿Por qué me afecta?**  
Puede revelar accesos a dominios maliciosos, descargas sospechosas y patrones de navegación asociados con actividad maliciosa.

**¿Cómo se soluciona?**  
Centralizando los registros, aplicando filtrado web y monitoreando dominios, URLs y patrones de tráfico sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comunicarse mediante servicios web legítimos o utilizar técnicas de evasión para dificultar la identificación de su tráfico.

## DNS Log

**¿Qué es?**  
DNS Log es un registro de las consultas y respuestas DNS procesadas por un servidor o resolver.

**¿Dónde lo encuentro?**  
En servidores DNS, resolvers, firewalls, sistemas de seguridad y SIEM.

**¿Por qué me afecta?**  
Puede revelar dominios maliciosos, reconocimiento de infraestructura, comunicaciones C2 y posibles intentos de DNS tunneling.

**¿Cómo se soluciona?**  
Monitoreando consultas, bloqueando dominios maliciosos y detectando patrones anómalos de resolución.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar DNS para localizar servidores C2 o transportar información mediante consultas especialmente construidas.

## Authentication Log

**¿Qué es?**  
Authentication Log es un registro de eventos relacionados con intentos y resultados de autenticación de usuarios o servicios.

**¿Dónde lo encuentro?**  
En sistemas operativos, Active Directory, aplicaciones, VPN, servicios cloud y sistemas de autenticación.

**¿Por qué me afecta?**  
Permite identificar accesos exitosos, intentos fallidos, ataques de fuerza bruta y uso sospechoso de credenciales.

**¿Cómo se soluciona?**  
Centralizando los registros, monitoreando patrones de autenticación y aplicando MFA, políticas de acceso y controles de cuenta.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas para autenticarse legítimamente y dificultar la distinción entre actividad maliciosa y acceso normal.

## Windows Event Log

**¿Qué es?**  
Windows Event Log es el sistema de registro de eventos de Windows que almacena información generada por el sistema operativo, aplicaciones y servicios.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows, normalmente mediante Event Viewer y otros sistemas de recopilación de logs.

**¿Por qué me afecta?**  
Contiene evidencia sobre autenticaciones, procesos, cambios del sistema, errores y otras actividades relevantes para una investigación.

**¿Cómo se soluciona?**  
Habilitando los eventos necesarios, protegiendo los registros y centralizándolos para su análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar, modificar o evitar eventos para reducir la evidencia disponible sobre sus actividades.

## Sysmon Log

**¿Qué es?**  
Sysmon Log es un registro generado por Sysmon que proporciona telemetría detallada sobre procesos, conexiones de red, archivos y otras actividades del sistema Windows.

**¿Dónde lo encuentro?**  
En endpoints Windows donde Sysmon está instalado y configurado, además de plataformas SIEM o EDR que recopilan sus eventos.

**¿Por qué me afecta?**  
Proporciona visibilidad adicional sobre comportamientos que pueden ser relevantes para detectar malware, ejecución de comandos y movimiento lateral.

**¿Cómo se soluciona?**  
Instalando Sysmon con una configuración adecuada, centralizando sus eventos y creando detecciones basadas en la telemetría disponible.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar deshabilitar Sysmon, evadir su configuración o modificar su comportamiento para reducir la telemetría generada.

## Application Log

**¿Qué es?**  
Application Log es un registro que contiene eventos generados por aplicaciones y servicios relacionados con su funcionamiento o errores.

**¿Dónde lo encuentro?**  
En servidores, estaciones de trabajo, aplicaciones empresariales y sistemas de monitoreo.

**¿Por qué me afecta?**  
Puede proporcionar evidencia sobre errores, accesos, operaciones y comportamientos anómalos dentro de una aplicación.

**¿Cómo se soluciona?**  
Habilitando registros relevantes, protegiéndolos y centralizándolos para facilitar su análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar una aplicación vulnerable y posteriormente intentar eliminar o manipular los registros que evidencien sus acciones.

## Security Log

**¿Qué es?**  
Security Log es un registro dedicado a eventos relacionados con la seguridad del sistema, como autenticaciones, uso de privilegios y cambios relevantes.

**¿Dónde lo encuentro?**  
Principalmente en sistemas Windows y entornos donde los eventos de seguridad son recopilados y enviados a un SIEM.

**¿Por qué me afecta?**  
Puede proporcionar evidencia sobre accesos sospechosos, abuso de privilegios y actividades relacionadas con cuentas.

**¿Cómo se soluciona?**  
Configurando auditoría adecuada, protegiendo los registros y centralizándolos para su monitoreo y análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar eventos, manipular configuraciones de auditoría o utilizar técnicas que reduzcan la evidencia registrada.

## System Log

**¿Qué es?**  
System Log es un registro que contiene eventos relacionados con el funcionamiento del sistema operativo y sus componentes.

**¿Dónde lo encuentro?**  
En sistemas operativos, servidores, endpoints y plataformas centralizadas de logging.

**¿Por qué me afecta?**  
Puede revelar fallos, cambios de servicios, problemas de controladores y otros eventos que ayuden a identificar actividad anómala.

**¿Cómo se soluciona?**  
Recopilando los eventos relevantes, protegiendo los registros y correlacionándolos con otras fuentes de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede provocar o aprovechar cambios en servicios y componentes del sistema y posteriormente intentar ocultar la evidencia generada.
