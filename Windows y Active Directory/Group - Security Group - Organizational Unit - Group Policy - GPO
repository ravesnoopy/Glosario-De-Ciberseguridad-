# Group

**¿Qué es?**  
Group es un conjunto de usuarios, equipos u otros objetos utilizado para administrar permisos y acceso a recursos de forma colectiva.

**¿Dónde lo encuentro?**  
En Active Directory, sistemas Windows, aplicaciones empresariales y otros entornos que utilizan grupos para gestionar el acceso.

**¿Por qué me afecta?**  
Una membresía incorrecta puede otorgar a un usuario permisos sobre información, sistemas o funciones que no debería poder utilizar.

**¿Cómo se soluciona?**  
Revisando periódicamente las membresías, aplicando mínimo privilegio y eliminando usuarios o equipos que ya no necesiten pertenecer al grupo.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar grupos privilegiados y sus miembros para descubrir posibles rutas de escalada de privilegios.

---

# Security Group

**¿Qué es?**  
Security Group es un grupo utilizado específicamente para asignar permisos y controlar el acceso a recursos dentro de Windows o Active Directory.

**¿Dónde lo encuentro?**  
En Active Directory, sistemas Windows, recursos compartidos, aplicaciones y otros servicios que utilizan grupos de seguridad.

**¿Por qué me afecta?**  
Los permisos asignados a un Security Group se aplican a sus miembros, por lo que una membresía incorrecta puede ampliar considerablemente el acceso de una cuenta.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, revisando membresías y permisos y controlando cuidadosamente los grupos administrativos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar comprometer una cuenta perteneciente a un grupo privilegiado o modificar membresías si obtiene permisos administrativos.

---

# Organizational Unit

**¿Qué es?**  
Organizational Unit (OU) es un contenedor de Active Directory utilizado para organizar usuarios, equipos, grupos y otros objetos y facilitar su administración.

**¿Dónde lo encuentro?**  
Dentro de la estructura jerárquica de un dominio de Active Directory.

**¿Por qué me afecta?**  
Las OUs permiten aplicar y organizar políticas administrativas. Una configuración incorrecta puede afectar a numerosos objetos simultáneamente.

**¿Cómo se soluciona?**  
Diseñando una estructura de OUs coherente, aplicando correctamente las políticas y revisando las delegaciones administrativas y permisos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar OUs con permisos o delegaciones excesivas para identificar oportunidades de escalada de privilegios o modificación de políticas.

---

# Group Policy

**¿Qué es?**  
Group Policy es un mecanismo de Windows y Active Directory que permite administrar y aplicar configuraciones de seguridad y funcionamiento a usuarios y equipos de forma centralizada.

**¿Dónde lo encuentro?**  
En entornos Windows administrados mediante Active Directory, donde las políticas pueden aplicarse a usuarios y equipos del dominio.

**¿Por qué me afecta?**  
Una política incorrecta puede modificar configuraciones de seguridad en numerosos equipos y crear debilidades a escala del dominio.

**¿Cómo se soluciona?**  
Aplicando configuraciones seguras, siguiendo una Security Baseline, controlando quién puede modificar las políticas y revisando periódicamente su configuración.

**¿Cómo lo usaría un atacante en mi contra?**  
Si obtiene privilegios suficientes, puede intentar modificar políticas para debilitar controles de seguridad o distribuir configuraciones maliciosas.

---

# GPO

**¿Qué es?**  
GPO (Group Policy Object) es un objeto que contiene configuraciones de Group Policy que pueden aplicarse a usuarios y equipos de Active Directory.

**¿Dónde lo encuentro?**  
En Active Directory y en los mecanismos de administración de Group Policy de Windows.

**¿Por qué me afecta?**  
Una GPO puede aplicar configuraciones a numerosos sistemas, por lo que una modificación no autorizada puede tener un impacto amplio.

**¿Cómo se soluciona?**  
Restringiendo los permisos de modificación, revisando el contenido y alcance de las GPO y monitoreando cambios administrativos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar modificar una GPO para cambiar configuraciones de seguridad, ejecutar acciones en múltiples equipos o establecer persistencia dentro del dominio.
