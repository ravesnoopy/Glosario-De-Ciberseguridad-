
## Logon Type

**¿Qué es?**  
Valor que identifica el tipo de inicio de sesión realizado en Windows, como interactivo, de red, remoto o mediante un servicio.

**¿Dónde lo encuentro?**  
En eventos de autenticación de Windows, especialmente en los registros de seguridad y herramientas SIEM.

**¿Por qué me afecta?**  
Permite determinar cómo se autenticó una cuenta y detectar patrones de acceso inusuales o incompatibles con el comportamiento esperado.

**¿Cómo se soluciona?**  
Monitorear los tipos de inicio de sesión y establecer detecciones para combinaciones anómalas de usuario, equipo, horario y tipo de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar credenciales comprometidas mediante distintos tipos de acceso para moverse lateralmente o acceder remotamente a sistemas.


## Logon ID

**¿Qué es?**  
Identificador asociado a una sesión de inicio de sesión en Windows que permite relacionar diferentes eventos con una misma autenticación.

**¿Dónde lo encuentro?**  
En eventos de seguridad de Windows y registros centralizados en herramientas SIEM.

**¿Por qué me afecta?**  
Facilita la correlación de eventos y permite reconstruir las acciones realizadas durante una sesión específica.

**¿Cómo se soluciona?**  
Conservar y correlacionar correctamente los eventos que contienen el Logon ID durante las investigaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Sus actividades podrían quedar relacionadas mediante el mismo identificador, permitiendo al analista reconstruir acciones realizadas durante una sesión comprometida.


## Session ID

**¿Qué es?**  
Identificador utilizado para distinguir una sesión activa o contexto de comunicación dentro de un sistema o aplicación.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, servicios remotos, servidores y registros de actividad.

**¿Por qué me afecta?**  
Permite relacionar acciones con una sesión específica y ayuda a identificar accesos simultáneos o comportamientos anómalos.

**¿Cómo se soluciona?**  
Registrar y proteger correctamente los identificadores de sesión y monitorear sesiones concurrentes o inesperadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar obtener o abusar de un identificador de sesión válido para actuar como una sesión legítima.


## Security Identifier

**¿Qué es?**  
Identificador único utilizado por Windows para representar entidades de seguridad, como usuarios, grupos y cuentas.

**¿Dónde lo encuentro?**  
En Active Directory, cuentas de Windows, permisos de archivos, procesos, eventos de seguridad y configuraciones del sistema.

**¿Por qué me afecta?**  
Los permisos de Windows se relacionan con estos identificadores, por lo que su análisis ayuda a determinar qué identidad realizó una acción y qué privilegios posee.

**¿Cómo se soluciona?**  
Administrar correctamente las cuentas, aplicar mínimo privilegio y revisar permisos y asociaciones de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar una identidad con privilegios excesivos o comprometida para realizar acciones autorizadas para ese Security Identifier.


## SID

**¿Qué es?**  
Security Identifier es el identificador único que Windows asigna a una cuenta, grupo u otra entidad de seguridad.

**¿Dónde lo encuentro?**  
En cuentas locales y de dominio, permisos NTFS, registros de Windows, Active Directory y eventos de seguridad.

**¿Por qué me afecta?**  
Permite determinar qué identidad está asociada con una acción o permiso, incluso cuando el nombre de la cuenta cambia.

**¿Cómo se soluciona?**  
Gestionar adecuadamente las identidades y privilegios y revisar permisos asociados a los SID relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar aprovechar cuentas con privilegios elevados o manipular configuraciones relacionadas con identidades para obtener mayores permisos.


## GUID

**¿Qué es?**  
Globally Unique Identifier es un identificador diseñado para distinguir de forma prácticamente única objetos, recursos o eventos dentro de diferentes sistemas.

**¿Dónde lo encuentro?**  
En Windows, Active Directory, aplicaciones, bases de datos, registros y servicios que necesitan identificar objetos de manera única.

**¿Por qué me afecta?**  
Permite correlacionar objetos y eventos incluso cuando sus nombres pueden cambiar o no ser suficientes para identificarlos.

**¿Cómo se soluciona?**  
Mantener los identificadores y registros necesarios para facilitar la correlación y trazabilidad durante las investigaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar objetos legítimos identificados mediante GUID durante una intrusión para interactuar con recursos sin depender únicamente de sus nombres.


## Correlation ID

**¿Qué es?**  
Identificador utilizado para relacionar múltiples eventos o solicitudes que forman parte de una misma operación o transacción.

**¿Dónde lo encuentro?**  
En aplicaciones, APIs, servicios distribuidos, sistemas cloud, logs y plataformas SIEM.

**¿Por qué me afecta?**  
Facilita reconstruir una actividad que atraviesa varios componentes y permite conectar eventos que individualmente podrían parecer aislados.

**¿Cómo se soluciona?**  
Generar, conservar y registrar correctamente los identificadores de correlación en los diferentes componentes de una arquitectura.

**¿Cómo lo usaría un atacante en mi contra?**  
Sus acciones pueden quedar vinculadas mediante un Correlation ID, permitiendo identificar la secuencia de solicitudes asociadas con una actividad maliciosa.


## Event Correlation

**¿Qué es?**  
Proceso de relacionar eventos provenientes de diferentes fuentes para identificar una actividad, secuencia o comportamiento que no sería evidente al analizar cada evento por separado.

**¿Dónde lo encuentro?**  
En SIEM, SOC, sistemas de monitoreo, EDR y plataformas de análisis de seguridad.

**¿Por qué me afecta?**  
Permite detectar ataques combinando señales como autenticaciones, procesos, conexiones de red y modificaciones de archivos.

**¿Cómo se soluciona?**  
Centralizar logs, normalizar eventos y crear reglas de correlación basadas en contexto y comportamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría distribuir sus acciones entre diferentes sistemas, cuentas y periodos para dificultar que los eventos sean correlacionados como parte de un mismo ataque.


## Timeline

**¿Qué es?**  
Representación cronológica de eventos que permite reconstruir la secuencia temporal de actividades ocurridas durante una operación o incidente.

**¿Dónde lo encuentro?**  
En investigaciones forenses, respuesta a incidentes, análisis de logs, SIEM y herramientas DFIR.

**¿Por qué me afecta?**  
Permite determinar qué ocurrió primero, cómo evolucionó un incidente y relacionar actividades de diferentes sistemas y fuentes.

**¿Cómo se soluciona?**  
Recopilar eventos con marcas de tiempo confiables, normalizar zonas horarias y correlacionar múltiples fuentes de evidencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría borrar o alterar evidencias y distribuir sus acciones temporalmente para dificultar la reconstrucción de la secuencia del ataque.
