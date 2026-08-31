# DLL

**¿Qué es?**  
DLL (Dynamic Link Library) es un archivo que contiene código y recursos que pueden ser utilizados por uno o varios programas de Windows.

**¿Dónde lo encuentro?**  
En sistemas Windows, aplicaciones, servicios y directorios que contienen componentes necesarios para ejecutar programas.

**¿Por qué me afecta?**  
Una DLL maliciosa o cargada de forma insegura puede permitir que código no autorizado se ejecute dentro del contexto de un proceso legítimo.

**¿Cómo se soluciona?**  
Manteniendo el software actualizado, controlando las rutas de carga de DLL, aplicando controles de integridad y evitando que aplicaciones carguen bibliotecas desde ubicaciones no confiables.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar reemplazar, cargar o hacer que un proceso legítimo utilice una DLL controlada por él para ejecutar código.

---

# EXE

**¿Qué es?**  
EXE es la extensión utilizada habitualmente por los archivos ejecutables de Windows que contienen instrucciones que pueden ser ejecutadas por el sistema operativo.

**¿Dónde lo encuentro?**  
En aplicaciones, herramientas, instaladores, servicios y otros componentes ejecutables de Windows.

**¿Por qué me afecta?**  
Un archivo EXE malicioso puede ejecutar código no autorizado cuando un usuario o proceso lo inicia.

**¿Cómo se soluciona?**  
Aplicando controles de ejecución, EDR/antivirus, listas de aplicaciones permitidas, gestión de privilegios y validación del origen de los ejecutables.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar un ejecutable malicioso o abusar de un programa legítimo para ejecutar acciones dentro del sistema comprometido.

---

# PowerShell

**¿Qué es?**  
PowerShell es una plataforma de automatización y administración de Windows que permite ejecutar comandos y scripts mediante una interfaz de línea de comandos.

**¿Dónde lo encuentro?**  
En sistemas Windows, servidores, estaciones de trabajo y entornos administrativos.

**¿Por qué me afecta?**  
PowerShell es una herramienta legítima con capacidades avanzadas que también pueden ser abusadas para ejecutar acciones maliciosas utilizando herramientas disponibles en el sistema.

**¿Cómo se soluciona?**  
Monitoreando la ejecución de PowerShell, aplicando políticas de seguridad, restringiendo su uso cuando sea necesario y registrando comandos y eventos relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede abusar de PowerShell para ejecutar scripts, automatizar acciones, recopilar información o interactuar con otros componentes del sistema sin necesidad de introducir herramientas adicionales.

---

# CMD

**¿Qué es?**  
CMD es el intérprete de comandos de Windows que permite ejecutar comandos y programas mediante una interfaz de línea de comandos.

**¿Dónde lo encuentro?**  
En sistemas operativos Windows, servidores y estaciones de trabajo.

**¿Por qué me afecta?**  
Puede utilizarse legítimamente para administración, pero también puede ser abusado para ejecutar comandos y automatizar acciones maliciosas.

**¿Cómo se soluciona?**  
Monitoreando procesos y líneas de comandos, aplicando mínimo privilegio y restringiendo su uso cuando las necesidades operativas lo permitan.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar CMD para ejecutar comandos, iniciar otros programas, modificar configuraciones o automatizar actividades dentro de un sistema comprometido.

---

# Windows Terminal

**¿Qué es?**  
Windows Terminal es una aplicación de Windows que proporciona una interfaz para utilizar diferentes shells e intérpretes de comandos, como PowerShell y CMD.

**¿Dónde lo encuentro?**  
En sistemas Windows modernos utilizados para administración y ejecución de herramientas de línea de comandos.

**¿Por qué me afecta?**  
Proporciona acceso a múltiples shells desde una misma interfaz, por lo que puede formar parte de actividades administrativas legítimas o de una investigación de seguridad.

**¿Cómo se soluciona?**  
Controlando qué usuarios pueden ejecutar herramientas administrativas, monitoreando los procesos iniciados desde Terminal y aplicando políticas de seguridad adecuadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar Windows Terminal como interfaz para ejecutar PowerShell, CMD u otros shells disponibles después de obtener acceso al sistema.
