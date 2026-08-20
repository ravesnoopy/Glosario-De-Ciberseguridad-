
## Sysmon

**¿Qué es?**  
Sysmon (System Monitor) es una herramienta de Windows que registra información detallada sobre procesos, conexiones de red, archivos y otras actividades del sistema para mejorar la visibilidad de seguridad.

**¿Dónde lo encuentro?**  
En endpoints y servidores Windows donde Sysmon está instalado y configurado, así como en plataformas SIEM que recopilan sus eventos.

**¿Por qué me afecta?**  
Proporciona telemetría detallada que puede ayudar a detectar ejecución de malware, procesos sospechosos, conexiones de red y otras actividades asociadas con ataques.

**¿Cómo se soluciona?**  
Instalando Sysmon con una configuración adecuada, centralizando sus eventos y creando detecciones basadas en la telemetría disponible.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evadir la telemetría, deshabilitar Sysmon o modificar su comportamiento para reducir los eventos que genera.

## Event Viewer

**¿Qué es?**  
Event Viewer es una herramienta de Windows que permite visualizar, filtrar y analizar eventos registrados por el sistema operativo, aplicaciones y servicios.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows mediante la herramienta `Event Viewer` o `eventvwr.msc`.

**¿Por qué me afecta?**  
Permite a los analistas revisar eventos relacionados con autenticaciones, errores, servicios y otras actividades que pueden proporcionar evidencia durante una investigación.

**¿Cómo se soluciona?**  
Manteniendo habilitados los registros relevantes, configurando políticas de auditoría adecuadas y centralizando los eventos para su análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar o manipular los registros para eliminar evidencia de sus actividades y dificultar una investigación.

## Windows Event Log

**¿Qué es?**  
Windows Event Log es el sistema de registro de Windows que almacena eventos generados por el sistema operativo, aplicaciones y servicios.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows, donde los eventos pueden consultarse mediante Event Viewer o recopilarse mediante herramientas de seguridad y SIEM.

**¿Por qué me afecta?**  
Contiene evidencia sobre autenticaciones, procesos, cambios de configuración, errores y otras actividades relevantes para detectar e investigar incidentes.

**¿Cómo se soluciona?**  
Configurando correctamente la auditoría, protegiendo los registros, estableciendo una retención adecuada y centralizando los eventos críticos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar eliminar eventos, modificar configuraciones de auditoría o evitar generar registros para dificultar la detección y el análisis forense.
