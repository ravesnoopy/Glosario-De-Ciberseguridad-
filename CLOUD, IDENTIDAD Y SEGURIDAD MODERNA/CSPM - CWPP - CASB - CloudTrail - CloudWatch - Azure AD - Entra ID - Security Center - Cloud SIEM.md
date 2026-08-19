
## CSPM

**¿Qué es?**  
Cloud Security Posture Management es una categoría de herramientas que evalúa continuamente la configuración de recursos cloud para identificar riesgos, incumplimientos y configuraciones inseguras.

**¿Dónde lo encuentro?**  
En plataformas de seguridad cloud que analizan servicios, identidades, redes, almacenamiento y configuraciones de proveedores cloud.

**¿Por qué me afecta?**  
Una configuración incorrecta puede exponer datos, servicios o identidades sin necesidad de explotar una vulnerabilidad de software.

**¿Cómo se soluciona?**  
Corregir configuraciones inseguras, aplicar políticas de seguridad, mínimo privilegio y monitoreo continuo de la postura cloud.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría recursos expuestos, permisos excesivos o configuraciones débiles para encontrar una vía de acceso al entorno cloud.


## CWPP

**¿Qué es?**  
Cloud Workload Protection Platform es una categoría de seguridad destinada a proteger cargas de trabajo cloud, como máquinas virtuales, contenedores y otros recursos de cómputo.

**¿Dónde lo encuentro?**  
En entornos cloud donde existen cargas de trabajo que necesitan protección contra malware, vulnerabilidades, comportamientos sospechosos y amenazas de ejecución.

**¿Por qué me afecta?**  
Una carga de trabajo comprometida puede convertirse en un punto de entrada para acceder a otros recursos dentro del entorno cloud.

**¿Cómo se soluciona?**  
Mantener cargas actualizadas, aplicar mínimo privilegio, proteger los endpoints y contenedores y monitorear comportamientos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer una carga de trabajo vulnerable y utilizarla como punto de entrada para ejecutar acciones o alcanzar otros recursos.


## CASB

**¿Qué es?**  
Cloud Access Security Broker es una capa de seguridad que ayuda a controlar y supervisar el uso de servicios cloud por parte de usuarios y organizaciones.

**¿Dónde lo encuentro?**  
En organizaciones que utilizan múltiples aplicaciones y servicios cloud y necesitan aplicar políticas de seguridad sobre el acceso y uso de estos servicios.

**¿Por qué me afecta?**  
El uso no controlado de servicios cloud puede provocar exposición de información, acceso no autorizado o transferencia de datos fuera de los controles corporativos.

**¿Cómo se soluciona?**  
Aplicar políticas de acceso, controlar aplicaciones cloud autorizadas, monitorear actividad y establecer controles de protección de datos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar una cuenta comprometida para utilizar servicios cloud autorizados y acceder o transferir información sin generar un patrón claramente malicioso.


## CloudTrail

**¿Qué es?**  
Servicio de AWS que registra actividades y llamadas realizadas mediante la consola, APIs, SDKs y otros componentes de una cuenta cloud.

**¿Dónde lo encuentro?**  
En entornos de Amazon Web Services donde se utiliza para auditoría, investigación de incidentes y monitoreo de actividad administrativa.

**¿Por qué me afecta?**  
Proporciona evidencia importante sobre quién realizó una acción, qué recurso fue afectado y cuándo ocurrió, siendo fundamental para investigar compromisos cloud.

**¿Cómo se soluciona?**  
Configurar el registro de actividad de forma adecuada, proteger los logs contra modificaciones o eliminación y centralizarlos para su análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Tras comprometer una identidad cloud, podría realizar acciones administrativas y posteriormente intentar eliminar, modificar o evitar los registros que evidencien su actividad.


## CloudWatch

**¿Qué es?**  
Servicio de AWS para monitorear métricas, logs, eventos y el comportamiento de recursos y aplicaciones dentro del entorno cloud.

**¿Dónde lo encuentro?**  
En infraestructuras AWS que necesitan supervisar aplicaciones, servidores, servicios, rendimiento y eventos operativos.

**¿Por qué me afecta?**  
Los datos de monitoreo pueden revelar actividad anómala, errores, cambios inesperados o indicadores relacionados con un incidente de seguridad.

**¿Cómo se soluciona?**  
Configurar métricas y alertas relevantes, centralizar logs, proteger su acceso y establecer reglas para detectar comportamientos anómalos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría operar de manera que su actividad genere el menor número posible de señales o, si obtiene privilegios suficientes, interferir con los mecanismos de monitoreo.


## Azure AD

**¿Qué es?**  
Azure Active Directory era el nombre anterior del servicio de identidad y acceso de Microsoft para gestionar usuarios, aplicaciones, dispositivos y autenticación en entornos cloud.

**¿Dónde lo encuentro?**  
En organizaciones que utilizan servicios de identidad de Microsoft; actualmente el servicio se denomina Microsoft Entra ID.

**¿Por qué me afecta?**  
Una cuenta comprometida puede proporcionar acceso a múltiples aplicaciones y recursos cloud dependiendo de sus permisos y relaciones de confianza.

**¿Cómo se soluciona?**  
Utilizar MFA, mínimo privilegio, políticas de acceso condicional, protección de identidades y monitoreo de autenticaciones y actividades administrativas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer una identidad mediante credenciales robadas, phishing u otros métodos para acceder posteriormente a recursos asociados a esa cuenta.


## Entra ID

**¿Qué es?**  
Microsoft Entra ID es el servicio de identidad y gestión de acceso de Microsoft para usuarios, aplicaciones, dispositivos y recursos cloud.

**¿Dónde lo encuentro?**  
En organizaciones que utilizan Microsoft 365, Azure y otras aplicaciones integradas con el ecosistema de identidad de Microsoft.

**¿Por qué me afecta?**  
La identidad se convierte en un componente crítico de seguridad cloud; el compromiso de una cuenta con privilegios elevados puede afectar numerosos recursos.

**¿Cómo se soluciona?**  
Aplicar MFA, acceso condicional, mínimo privilegio, protección de identidades, administración segura de cuentas privilegiadas y monitoreo de autenticaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer una identidad y utilizar sus permisos para acceder a aplicaciones, datos o recursos cloud autorizados para esa cuenta.


## Security Center

**¿Qué es?**  
Nombre utilizado históricamente por Microsoft para sus capacidades de evaluación y protección de seguridad en Azure; actualmente estas capacidades forman parte principalmente de Microsoft Defender for Cloud.

**¿Dónde lo encuentro?**  
En entornos Microsoft Azure y en herramientas de seguridad destinadas a evaluar la postura y protección de recursos cloud.

**¿Por qué me afecta?**  
Ayuda a identificar configuraciones inseguras, vulnerabilidades y amenazas que podrían permitir el compromiso de recursos cloud.

**¿Cómo se soluciona?**  
Habilitar las recomendaciones de seguridad relevantes, corregir configuraciones inseguras, proteger cargas de trabajo y mantener una supervisión continua del entorno.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría recursos con configuraciones débiles o vulnerabilidades que le permitan obtener acceso inicial o ampliar su presencia dentro del entorno.


## Cloud SIEM

**¿Qué es?**  
Sistema de gestión de información y eventos de seguridad adaptado a entornos cloud que centraliza, correlaciona y analiza registros y señales de seguridad de múltiples fuentes.

**¿Dónde lo encuentro?**  
En centros de operaciones de seguridad que monitorean infraestructuras cloud, aplicaciones, identidades, endpoints, redes y servicios.

**¿Por qué me afecta?**  
Permite correlacionar eventos distribuidos y detectar patrones de ataque que podrían pasar desapercibidos al analizar cada fuente de manera aislada.

**¿Cómo se soluciona?**  
Centralizar logs relevantes, configurar reglas de detección, mantener fuentes de datos completas y ajustar alertas para reducir falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría evadir las detecciones generando actividad que parezca legítima, utilizando cuentas comprometidas o reduciendo las señales que permitan correlacionar sus acciones.
