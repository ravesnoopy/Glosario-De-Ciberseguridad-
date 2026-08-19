
## Acquisition

**¿Qué es?**  
Acquisition es el proceso de recopilar y preservar datos digitales de un sistema para su posterior análisis forense, procurando mantener su integridad y trazabilidad.

**¿Dónde lo encuentro?**  
En investigaciones DFIR, análisis de incidentes y procesos forenses que requieren recolectar discos, memoria, registros, archivos u otras evidencias digitales.

**¿Por qué me afecta?**  
Una adquisición incorrecta puede alterar o destruir evidencia relevante y dificultar la reconstrucción de las acciones realizadas durante un incidente.

**¿Cómo se soluciona?**  
Utilizando procedimientos documentados, herramientas forenses apropiadas, mecanismos de verificación de integridad y una cadena de custodia adecuada.

**¿Cómo lo usaría un atacante en mi contra?**  
Un atacante puede intentar eliminar, modificar o cifrar información antes de su adquisición para dificultar la investigación y ocultar sus actividades.

## Disk Image

**¿Qué es?**  
Una Disk Image es una copia forense de un medio de almacenamiento que conserva los datos y estructuras relevantes del dispositivo para su análisis.

**¿Dónde lo encuentro?**  
En investigaciones forenses de discos duros, SSD, dispositivos externos y otros medios de almacenamiento.

**¿Por qué me afecta?**  
Permite analizar un sistema sin trabajar directamente sobre el dispositivo original y puede contener evidencia como archivos eliminados, metadatos y artefactos del sistema.

**¿Cómo se soluciona?**  
Realizando la adquisición con herramientas forenses, verificando la integridad mediante hashes y preservando correctamente la evidencia original.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar eliminar archivos, modificar timestamps o destruir información antes de que el dispositivo sea adquirido para dificultar el análisis.

## Memory Dump

**¿Qué es?**  
Un Memory Dump es una captura del contenido de la memoria RAM de un sistema en un momento determinado.

**¿Dónde lo encuentro?**  
En investigaciones de sistemas comprometidos donde se necesita analizar procesos, conexiones, credenciales, malware u otra información presente en memoria.

**¿Por qué me afecta?**  
La memoria puede contener información que no existe en el disco, incluyendo procesos maliciosos, conexiones activas y material sensible utilizado durante un ataque.

**¿Cómo se soluciona?**  
Adquiriendo la memoria lo antes posible cuando sea relevante, preservando su integridad y analizándola con herramientas forenses especializadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede ejecutar malware exclusivamente en memoria o almacenar información sensible allí para reducir la evidencia persistente en disco.

## PCAP

**¿Qué es?**  
PCAP es un formato utilizado para almacenar capturas de tráfico de red, incluyendo paquetes intercambiados entre sistemas durante un período determinado.

**¿Dónde lo encuentro?**  
En herramientas de captura de tráfico, sensores de red, sistemas de monitoreo y análisis forense de comunicaciones.

**¿Por qué me afecta?**  
Puede revelar conexiones sospechosas, protocolos utilizados, transferencias de datos y patrones de comunicación asociados con un ataque.

**¿Cómo se soluciona?**  
Capturando el tráfico relevante, protegiendo los archivos PCAP y analizándolos junto con otras fuentes de evidencia para identificar actividad maliciosa.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar ocultar sus comunicaciones mediante cifrado, protocolos permitidos o canales que dificulten distinguir el tráfico malicioso del legítimo.

## Registry Analysis

**¿Qué es?**  
Registry Analysis es el análisis forense del Windows Registry para identificar configuraciones, actividad del sistema y artefactos relacionados con usuarios, aplicaciones y mecanismos de persistencia.

**¿Dónde lo encuentro?**  
En investigaciones forenses de sistemas Windows, especialmente al analizar archivos y claves del registro asociados con actividad sospechosa.

**¿Por qué me afecta?**  
El registro puede contener evidencia de ejecución de programas, configuraciones modificadas, usuarios, dispositivos y mecanismos utilizados para mantener persistencia.

**¿Cómo se soluciona?**  
Analizando las colmenas relevantes de forma forense, correlacionando los hallazgos con otras evidencias y preservando los archivos originales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar claves del registro para establecer persistencia, alterar configuraciones de seguridad o dificultar la investigación de sus actividades.

## Event Log Analysis

**¿Qué es?**  
Event Log Analysis es el análisis de registros de eventos para identificar actividades, errores, cambios y comportamientos que puedan estar relacionados con un incidente de seguridad.

**¿Dónde lo encuentro?**  
En sistemas Windows, servidores, aplicaciones y plataformas centralizadas como SIEM que recopilan eventos de diferentes dispositivos.

**¿Por qué me afecta?**  
Los registros pueden proporcionar evidencia sobre inicios de sesión, creación de cuentas, ejecución de procesos, cambios de privilegios y otras acciones realizadas durante un ataque.

**¿Cómo se soluciona?**  
Centralizando registros, sincronizando el tiempo, estableciendo políticas de retención adecuadas y creando reglas para detectar eventos relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar, modificar o generar ruido en los registros para ocultar sus actividades y dificultar la reconstrucción de la línea temporal del ataque.
