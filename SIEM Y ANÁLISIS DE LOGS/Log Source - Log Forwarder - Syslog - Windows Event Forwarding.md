
## Log Source

**¿Qué es?**  
Log Source es el sistema, dispositivo, aplicación o servicio que genera registros sobre las actividades que ocurren en un entorno.

**¿Dónde lo encuentro?**  
En servidores, endpoints, firewalls, routers, aplicaciones, sistemas operativos, servicios cloud y dispositivos de seguridad.

**¿Por qué me afecta?**  
Los logs proporcionan evidencia necesaria para detectar amenazas, investigar incidentes y reconstruir actividades realizadas en un sistema.

**¿Cómo se soluciona?**  
Identificando las fuentes críticas, habilitando los registros necesarios y centralizándolos para facilitar su monitoreo y análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar deshabilitar, modificar o evitar los registros de una fuente para reducir la evidencia de sus actividades.

## Log Forwarder

**¿Qué es?**  
Log Forwarder es un componente que recopila registros de una o más fuentes y los envía hacia un sistema centralizado para almacenamiento o análisis.

**¿Dónde lo encuentro?**  
En endpoints, servidores, agentes de logging, plataformas SIEM y arquitecturas de monitoreo centralizado.

**¿Por qué me afecta?**  
Permite centralizar eventos de diferentes sistemas y facilita la detección y correlación de actividades sospechosas.

**¿Cómo se soluciona?**  
Protegiendo los agentes, verificando que los eventos se transmitan correctamente y monitoreando interrupciones o cambios inesperados en el flujo de logs.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar detener o manipular el componente de forwarding para impedir que determinadas actividades lleguen al SIEM.

## Syslog

**¿Qué es?**  
Syslog es un estándar utilizado para generar, transmitir y almacenar mensajes de registro provenientes de sistemas y dispositivos de red.

**¿Dónde lo encuentro?**  
En routers, firewalls, servidores Linux, aplicaciones y plataformas centralizadas de gestión de logs.

**¿Por qué me afecta?**  
Permite centralizar eventos de múltiples dispositivos y proporciona información útil para detectar accesos, errores y actividades sospechosas.

**¿Cómo se soluciona?**  
Configurando correctamente las fuentes, protegiendo la transmisión de logs y utilizando almacenamiento centralizado con controles de acceso y retención adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar generar grandes cantidades de eventos para dificultar el análisis o evitar que determinadas actividades queden registradas.

## Windows Event Forwarding

**¿Qué es?**  
Windows Event Forwarding (WEF) es una característica de Windows que permite recopilar y reenviar eventos de diferentes equipos hacia un servidor central.

**¿Dónde lo encuentro?**  
En entornos Windows empresariales donde se centralizan eventos de seguridad, sistema y aplicaciones para monitoreo o análisis.

**¿Por qué me afecta?**  
Permite recopilar eventos de múltiples equipos y mejorar la visibilidad de actividades relacionadas con autenticaciones, procesos y cambios en los sistemas.

**¿Cómo se soluciona?**  
Configurando correctamente los colectores y equipos origen, protegiendo las comunicaciones y verificando que los eventos críticos se reciban correctamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar deshabilitar servicios relacionados con el registro o modificar configuraciones para evitar que sus actividades sean enviadas al sistema central.
