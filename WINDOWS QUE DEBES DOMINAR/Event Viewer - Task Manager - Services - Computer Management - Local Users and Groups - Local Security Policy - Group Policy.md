# Event Viewer

**¿Qué es?**  
Event Viewer es una herramienta administrativa de Windows que permite visualizar y analizar eventos registrados por el sistema operativo, aplicaciones y servicios.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows, mediante `eventvwr.msc` o desde las herramientas administrativas del sistema.

**¿Por qué me afecta?**  
Permite revisar eventos relacionados con autenticaciones, errores, servicios, aplicaciones y otras actividades que pueden proporcionar evidencia de seguridad.

**¿Cómo se soluciona?**  
Manteniendo habilitados los registros relevantes, configurando correctamente la auditoría y centralizando los eventos importantes para su análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar registros o modificar configuraciones de auditoría para dificultar la detección y el análisis de sus actividades.

---

# Task Manager

**¿Qué es?**  
Task Manager es una herramienta de Windows que permite visualizar y administrar procesos, aplicaciones, servicios, rendimiento y otros recursos del sistema.

**¿Dónde lo encuentro?**  
En equipos Windows mediante Task Manager o `taskmgr.exe`.

**¿Por qué me afecta?**  
Permite identificar procesos que consumen recursos de forma anómala y observar aplicaciones o servicios actualmente ejecutándose.

**¿Cómo se soluciona?**  
Utilizando la información de procesos y servicios como parte de la administración y monitoreo del sistema, complementándola con herramientas de seguridad más completas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizarlo para identificar procesos de seguridad, servicios activos y otros componentes del sistema después de obtener acceso.

---

# Services

**¿Qué es?**  
Services es la administración de servicios de Windows que permite visualizar, iniciar, detener y configurar procesos que funcionan como servicios del sistema.

**¿Dónde lo encuentro?**  
En Windows mediante `services.msc` y otras herramientas administrativas.

**¿Por qué me afecta?**  
Los servicios pueden tener privilegios elevados y algunos son esenciales para el funcionamiento y la seguridad del sistema.

**¿Cómo se soluciona?**  
Revisando periódicamente los servicios instalados, deshabilitando los innecesarios y controlando los permisos y configuraciones de los servicios críticos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar abusar de servicios existentes, modificar su configuración o crear mecanismos que permitan ejecutar procesos de forma persistente.

---

# Computer Management

**¿Qué es?**  
Computer Management es una consola administrativa de Windows que reúne diferentes herramientas para gestionar usuarios, discos, servicios, eventos y otros componentes del sistema.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows mediante `compmgmt.msc`.

**¿Por qué me afecta?**  
Centraliza varias funciones administrativas que pueden modificar componentes importantes del sistema.

**¿Cómo se soluciona?**  
Limitando el acceso a cuentas administrativas, aplicando mínimo privilegio y monitoreando cambios realizados mediante herramientas administrativas.

**¿Cómo lo usaría un atacante en mi contra?**  
Si obtiene privilegios suficientes, puede utilizar sus componentes administrativos para modificar configuraciones, cuentas, servicios o recursos del sistema.

---

# Local Users and Groups

**¿Qué es?**  
Local Users and Groups es una herramienta de Windows utilizada para administrar las cuentas y grupos locales de un equipo.

**¿Dónde lo encuentro?**  
En sistemas Windows que incluyen esta consola, mediante `lusrmgr.msc`.

**¿Por qué me afecta?**  
Las cuentas locales pueden proporcionar acceso directo al sistema y los grupos determinan qué permisos tienen esas cuentas.

**¿Cómo se soluciona?**  
Eliminando cuentas innecesarias, aplicando mínimo privilegio, protegiendo las cuentas administrativas y revisando periódicamente las membresías de grupos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar crear, modificar o utilizar cuentas locales para mantener acceso o aumentar sus privilegios si obtiene los permisos necesarios.

---

# Local Security Policy

**¿Qué es?**  
Local Security Policy es una configuración de Windows que permite establecer políticas de seguridad locales relacionadas con autenticación, auditoría, privilegios y otros controles.

**¿Dónde lo encuentro?**  
En determinadas ediciones de Windows mediante `secpol.msc`.

**¿Por qué me afecta?**  
Una política de seguridad débil puede permitir contraseñas inseguras, configuraciones de auditoría insuficientes o asignaciones de privilegios excesivas.

**¿Cómo se soluciona?**  
Aplicando configuraciones de seguridad adecuadas, siguiendo una Security Baseline y revisando periódicamente las políticas configuradas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar aprovechar configuraciones débiles o modificar políticas si obtiene privilegios administrativos.

---

# Group Policy

**¿Qué es?**  
Group Policy es un mecanismo de Windows y Active Directory que permite administrar y aplicar configuraciones y políticas de forma centralizada a usuarios y equipos.

**¿Dónde lo encuentro?**  
En entornos Windows, especialmente aquellos administrados mediante Active Directory y Domain Controllers.

**¿Por qué me afecta?**  
Una configuración incorrecta de Group Policy puede afectar simultáneamente a numerosos usuarios y equipos y puede introducir debilidades de seguridad a gran escala.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, separando responsabilidades administrativas, revisando las políticas y utilizando configuraciones de seguridad estandarizadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Si obtiene privilegios suficientes, puede intentar modificar políticas para debilitar controles de seguridad o distribuir configuraciones maliciosas dentro del dominio.
