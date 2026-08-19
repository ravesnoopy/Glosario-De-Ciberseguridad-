
## API Gateway

**¿Qué es?**  
Servicio que actúa como punto de entrada para APIs, gestionando solicitudes entre clientes y los servicios backend correspondientes.

**¿Dónde lo encuentro?**  
En arquitecturas cloud y aplicaciones distribuidas que exponen APIs para aplicaciones web, móviles, microservicios o integraciones externas.

**¿Por qué me afecta?**  
Una configuración insegura puede exponer APIs, permitir accesos no autorizados, omitir controles de autenticación o facilitar abusos contra los servicios backend.

**¿Cómo se soluciona?**  
Aplicar autenticación y autorización, validación de solicitudes, límites de velocidad, registro de eventos y políticas restrictivas de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría endpoints expuestos o configuraciones débiles para acceder a funciones o datos que deberían estar restringidos.


## Load Balancer

**¿Qué es?**  
Componente que distribuye las solicitudes de red entre múltiples servidores o instancias para mejorar disponibilidad, rendimiento y tolerancia a fallos.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs y arquitecturas cloud con múltiples servidores o instancias que atienden el mismo servicio.

**¿Por qué me afecta?**  
Una configuración incorrecta puede exponer servicios internos, permitir tráfico no deseado o afectar la disponibilidad de toda la aplicación.

**¿Cómo se soluciona?**  
Configurar correctamente listeners, reglas de acceso, certificados, redes y grupos de seguridad, evitando exponer directamente los servidores backend cuando no sea necesario.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría analizar el balanceador como punto de entrada para identificar servicios expuestos, configuraciones débiles o rutas que permitan alcanzar componentes internos.


## Object Storage

**¿Qué es?**  
Modelo de almacenamiento diseñado para guardar datos como objetos, normalmente acompañados de metadatos y organizados en contenedores o estructuras equivalentes.

**¿Dónde lo encuentro?**  
En servicios cloud utilizados para almacenar archivos, respaldos, imágenes, documentos, registros y grandes volúmenes de datos.

**¿Por qué me afecta?**  
Una configuración incorrecta de permisos puede hacer que información sensible quede expuesta públicamente o sea accesible por identidades no autorizadas.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, bloquear acceso público cuando no sea necesario, utilizar cifrado, controlar políticas de acceso y monitorear operaciones sobre los objetos.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría contenedores o recursos expuestos y aprovecharía permisos incorrectos para consultar, modificar o extraer información.


## S3

**¿Qué es?**  
Amazon Simple Storage Service es un servicio de almacenamiento de objetos utilizado para guardar y recuperar datos mediante contenedores llamados buckets.

**¿Dónde lo encuentro?**  
En infraestructuras cloud que utilizan Amazon Web Services para almacenar archivos, respaldos, logs, aplicaciones y otros datos.

**¿Por qué me afecta?**  
Buckets o políticas de acceso configurados incorrectamente pueden exponer información sensible o permitir modificaciones no autorizadas.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, bloquear acceso público innecesario, utilizar políticas de bucket adecuadas, cifrado y monitoreo de accesos.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría buckets accesibles o credenciales con permisos excesivos para intentar descubrir, descargar o modificar información almacenada.


## Blob Storage

**¿Qué es?**  
Servicio de almacenamiento de objetos utilizado para guardar grandes cantidades de datos no estructurados, como archivos, imágenes, vídeos y respaldos.

**¿Dónde lo encuentro?**  
En plataformas cloud, especialmente en servicios de almacenamiento basados en blobs utilizados por aplicaciones y sistemas empresariales.

**¿Por qué me afecta?**  
Los contenedores, objetos o credenciales configurados incorrectamente pueden provocar exposición o modificación no autorizada de información.

**¿Cómo se soluciona?**  
Aplicar mínimo privilegio, restringir acceso público, utilizar controles de identidad, cifrado, políticas de acceso y monitoreo de operaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría identificar almacenamiento expuesto o credenciales con permisos excesivos para acceder o extraer información.


## Virtual Network

**¿Qué es?**  
Red lógica aislada dentro de una infraestructura cloud que permite organizar y controlar la comunicación entre recursos mediante subredes, rutas y controles de acceso.

**¿Dónde lo encuentro?**  
En arquitecturas cloud donde servidores, bases de datos, aplicaciones y otros recursos necesitan comunicarse de forma controlada.

**¿Por qué me afecta?**  
Una segmentación o configuración de rutas deficiente puede permitir que un atacante acceda desde un recurso comprometido hacia sistemas internos.

**¿Cómo se soluciona?**  
Segmentar recursos por función, controlar rutas y comunicaciones, limitar exposición a Internet y aplicar el principio de mínimo acceso entre redes.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de comprometer un recurso, podría utilizar la conectividad disponible dentro de la red para descubrir o alcanzar otros servicios internos.


## Security Group

**¿Qué es?**  
Conjunto de reglas que controla el tráfico permitido hacia o desde determinados recursos dentro de una infraestructura cloud.

**¿Dónde lo encuentro?**  
En recursos cloud como máquinas virtuales, servidores y otros componentes que requieren controles de tráfico a nivel de instancia o recurso.

**¿Por qué me afecta?**  
Reglas demasiado permisivas pueden exponer servicios innecesarios a Internet o permitir comunicaciones que faciliten el movimiento lateral.

**¿Cómo se soluciona?**  
Permitir únicamente los puertos, protocolos, orígenes y destinos necesarios, revisar periódicamente las reglas y evitar exposiciones amplias innecesarias.

**¿Cómo lo usaría un atacante en mi contra?**  
Buscaría recursos con reglas demasiado permisivas para identificar servicios accesibles desde Internet o desde otros sistemas comprometidos.


## Network ACL

**¿Qué es?**  
Lista de reglas que controla el tráfico de red permitido o denegado entre subredes o interfaces según las capacidades de la plataforma cloud.

**¿Dónde lo encuentro?**  
En redes virtuales cloud, donde se utiliza como una capa adicional de filtrado de tráfico a nivel de red o subred.

**¿Por qué me afecta?**  
Una ACL demasiado permisiva puede aumentar la superficie de ataque y permitir comunicaciones que deberían estar bloqueadas.

**¿Cómo se soluciona?**  
Definir reglas específicas según las necesidades de cada red, revisar periódicamente las excepciones y aplicar segmentación y mínimo acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Analizaría las comunicaciones permitidas para determinar qué sistemas o servicios internos pueden alcanzarse desde un recurso comprometido.


## Cloud Firewall

**¿Qué es?**  
Control de seguridad de red diseñado para inspeccionar y filtrar tráfico entre redes, recursos cloud o Internet según políticas de seguridad.

**¿Dónde lo encuentro?**  
En arquitecturas cloud que requieren controlar tráfico entrante, saliente o entre diferentes segmentos de red.

**¿Por qué me afecta?**  
Una política incorrecta puede permitir conexiones maliciosas, exponer servicios o facilitar comunicaciones de un sistema comprometido con infraestructura externa.

**¿Cómo se soluciona?**  
Aplicar políticas de mínimo acceso, controlar tráfico entrante y saliente, registrar eventos, revisar reglas periódicamente y bloquear comunicaciones innecesarias.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría identificar reglas permisivas para establecer comunicaciones con servicios comprometidos, alcanzar recursos internos o mantener comunicación con infraestructura externa.
