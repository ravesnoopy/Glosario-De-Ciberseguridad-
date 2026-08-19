
## Firewall Rule

**¿Qué es?**  
Regla de configuración que determina qué tráfico de red puede permitirse, bloquearse o registrarse según criterios como origen, destino, puerto o protocolo.

**¿Dónde lo encuentro?**  
En firewalls de red, firewalls de host, dispositivos de seguridad y entornos cloud.

**¿Por qué me afecta?**  
Una regla demasiado permisiva puede exponer servicios o permitir comunicaciones no autorizadas, mientras que una regla incorrecta puede interrumpir servicios legítimos.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, limitar origen y destino, revisar reglas periódicamente y eliminar excepciones innecesarias.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría reglas permisivas o mal configuradas que le permitan acceder a servicios, comunicarse con otros sistemas o mantener conexiones no autorizadas.


## Network Segmentation

**¿Qué es?**  
Estrategia que divide una red en diferentes segmentos para controlar y limitar la comunicación entre sistemas y recursos.

**¿Dónde lo encuentro?**  
En redes empresariales, centros de datos, entornos cloud, VLAN, subredes y arquitecturas de seguridad.

**¿Por qué me afecta?**  
Una segmentación adecuada limita el movimiento lateral y reduce el impacto de un sistema comprometido.

**¿Cómo se soluciona?**  
Separar recursos según su función y nivel de confianza y controlar estrictamente las comunicaciones entre segmentos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría aprovechar una segmentación débil o controles entre segmentos mal configurados para desplazarse hacia otros sistemas.


## DMZ

**¿Qué es?**  
Zona de red diseñada para alojar servicios que necesitan estar accesibles desde redes externas, manteniéndolos separados de la red interna.

**¿Dónde lo encuentro?**  
En arquitecturas empresariales donde se exponen servicios como servidores web, correo u otros recursos hacia Internet.

**¿Por qué me afecta?**  
Una DMZ correctamente diseñada limita el impacto de un compromiso de servicios expuestos, pero una configuración incorrecta puede permitir acceso hacia la red interna.

**¿Cómo se soluciona?**  
Aislar la DMZ, controlar estrictamente el tráfico entre zonas y evitar conexiones innecesarias hacia la red interna.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría comprometer un servicio expuesto en la DMZ y posteriormente intentar utilizarlo como punto de partida para acceder a recursos internos.


## Wireshark

**¿Qué es?**  
Herramienta de análisis de tráfico de red que permite capturar y examinar paquetes para investigar comunicaciones y comportamientos de red.

**¿Dónde lo encuentro?**  
En análisis de redes, troubleshooting, laboratorios, investigaciones forenses y respuesta a incidentes.

**¿Por qué me afecta?**  
Permite identificar conexiones sospechosas, protocolos utilizados, errores de comunicación y posibles indicadores de compromiso.

**¿Cómo se soluciona?**  
Utilizarlo para analizar tráfico relevante, correlacionar las capturas con otras fuentes y proteger las capturas obtenidas como evidencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar herramientas de captura de tráfico para observar comunicaciones accesibles y recopilar información útil sobre sistemas, protocolos o credenciales transmitidas sin protección.
