# Registry

**¿Qué es?**  
Registry es la base de datos jerárquica de Windows que almacena configuraciones del sistema operativo, aplicaciones, usuarios y componentes.

**¿Dónde lo encuentro?**  
En sistemas Windows, mediante herramientas como Registry Editor (`regedit`) y diferentes mecanismos de administración y análisis.

**¿Por qué me afecta?**  
Cambios en el Registry pueden modificar configuraciones importantes del sistema y también pueden proporcionar mecanismos de persistencia o alterar controles de seguridad.

**¿Cómo se soluciona?**  
Controlando los permisos de acceso, monitoreando modificaciones relevantes y realizando copias de seguridad de configuraciones críticas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar determinadas claves o valores para alterar configuraciones, establecer persistencia o debilitar controles de seguridad.

---

# Registry Key

**¿Qué es?**  
Registry Key es una estructura dentro del Windows Registry que funciona como un contenedor para organizar configuraciones y valores relacionados.

**¿Dónde lo encuentro?**  
En el Windows Registry, organizado en diferentes ramas y subclaves.

**¿Por qué me afecta?**  
Algunas Registry Keys controlan comportamientos importantes del sistema, aplicaciones y mecanismos de inicio automático.

**¿Cómo se soluciona?**  
Protegiendo las claves sensibles, restringiendo permisos y monitoreando cambios inesperados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar claves específicas para alterar configuraciones o establecer mecanismos de persistencia.

---

# Registry Value

**¿Qué es?**  
Registry Value es un dato almacenado dentro de una Registry Key que contiene información utilizada para configurar el comportamiento de Windows o de una aplicación.

**¿Dónde lo encuentro?**  
Dentro de las Registry Keys del Windows Registry.

**¿Por qué me afecta?**  
Un valor modificado puede cambiar el comportamiento de una aplicación, servicio o componente del sistema.

**¿Cómo se soluciona?**  
Monitoreando modificaciones de valores sensibles y aplicando controles de acceso adecuados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar valores para cambiar configuraciones, ejecutar componentes o establecer persistencia.

---

# File System

**¿Qué es?**  
File System es el conjunto de estructuras y mecanismos que utiliza un sistema operativo para organizar, almacenar y administrar archivos y directorios.

**¿Dónde lo encuentro?**  
En discos duros, SSD, dispositivos extraíbles y otros medios de almacenamiento.

**¿Por qué me afecta?**  
Los permisos y estructuras del sistema de archivos determinan quién puede acceder, modificar o ejecutar archivos.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, configurando correctamente los permisos y monitoreando cambios en archivos y directorios sensibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar archivos accesibles con permisos excesivos o modificar archivos si obtiene permisos suficientes.

---

# NTFS

**¿Qué es?**  
NTFS (New Technology File System) es el sistema de archivos utilizado principalmente por Windows para almacenar y administrar archivos y directorios.

**¿Dónde lo encuentro?**  
En volúmenes de almacenamiento utilizados por sistemas Windows.

**¿Por qué me afecta?**  
NTFS permite aplicar permisos detallados sobre archivos y directorios, por lo que una configuración incorrecta puede provocar accesos no autorizados.

**¿Cómo se soluciona?**  
Configurando correctamente los permisos NTFS, aplicando mínimo privilegio y revisando periódicamente las ACL.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar archivos o directorios cuyos permisos permitan modificar, ejecutar o acceder a información que debería estar restringida.

---

# File Permissions

**¿Qué es?**  
File Permissions son los permisos que determinan qué usuarios y grupos pueden realizar acciones sobre un archivo o directorio, como leer, modificar o ejecutar.

**¿Dónde lo encuentro?**  
En sistemas de archivos, especialmente NTFS en Windows.

**¿Por qué me afecta?**  
Permisos excesivos pueden permitir que usuarios o procesos modifiquen archivos críticos o accedan a información sensible.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, revisando permisos heredados y eliminando accesos innecesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar archivos con permisos débiles para modificar configuraciones, reemplazar componentes o acceder a información.

---

# ACL

**¿Qué es?**  
ACL (Access Control List) es una lista de reglas que define qué usuarios o grupos tienen determinados permisos sobre un recurso.

**¿Dónde lo encuentro?**  
En sistemas de archivos, objetos de Windows, redes, aplicaciones y otros sistemas que implementan control de acceso.

**¿Por qué me afecta?**  
Una ACL configurada incorrectamente puede conceder acceso a recursos a usuarios o procesos que no deberían tenerlo.

**¿Cómo se soluciona?**  
Revisando las entradas de control de acceso, aplicando mínimo privilegio y eliminando permisos innecesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar ACLs mal configuradas que le permitan acceder, modificar o controlar recursos.

---

# DACL

**¿Qué es?**  
DACL (Discretionary Access Control List) es la lista de permisos que determina qué usuarios o grupos tienen permitido o denegado el acceso a un objeto de Windows.

**¿Dónde lo encuentro?**  
En objetos de Windows, archivos, carpetas, servicios, claves del Registry y otros recursos protegibles.

**¿Por qué me afecta?**  
Una DACL incorrecta puede permitir que una cuenta tenga permisos superiores a los necesarios sobre un recurso.

**¿Cómo se soluciona?**  
Revisando las entradas de permisos, aplicando mínimo privilegio y controlando las delegaciones de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar permisos excesivos o delegaciones incorrectas para obtener acceso o modificar recursos protegidos.

---

# SACL

**¿Qué es?**  
SACL (System Access Control List) es la lista de auditoría asociada a un objeto de Windows que determina qué tipos de accesos deben generar eventos de auditoría.

**¿Dónde lo encuentro?**  
En archivos, carpetas, objetos del sistema, Registry y otros recursos de Windows compatibles con auditoría.

**¿Por qué me afecta?**  
Una SACL correctamente configurada permite generar evidencia sobre accesos a recursos importantes y facilita la detección de actividad sospechosa.

**¿Cómo se soluciona?**  
Configurando auditorías relevantes, evitando generar ruido innecesario y enviando los eventos importantes a sistemas centralizados de monitoreo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar realizar acciones que no sean auditadas o modificar configuraciones de auditoría si consigue privilegios suficientes.

---

# SID

**¿Qué es?**  
SID (Security Identifier) es un identificador único utilizado por Windows para identificar cuentas, grupos y otras entidades de seguridad.

**¿Dónde lo encuentro?**  
En sistemas Windows, Active Directory, perfiles de usuarios, ACLs y eventos de seguridad.

**¿Por qué me afecta?**  
Los SIDs permiten determinar qué identidad está asociada con permisos y actividades registradas en el sistema.

**¿Cómo se soluciona?**  
Administrando correctamente las cuentas y permisos y monitoreando cambios relacionados con identidades y grupos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede recopilar SIDs durante el reconocimiento del entorno y utilizarlos para comprender identidades, permisos y relaciones dentro del sistema o dominio.
