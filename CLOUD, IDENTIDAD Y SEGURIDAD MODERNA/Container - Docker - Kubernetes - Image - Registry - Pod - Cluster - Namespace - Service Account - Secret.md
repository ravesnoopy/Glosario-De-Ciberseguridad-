
## Container

**¿Qué es?**  
Un Container es un entorno aislado que empaqueta una aplicación junto con sus dependencias para ejecutarla de forma consistente sobre un sistema operativo compartido.

**¿Dónde lo encuentro?**  
En servidores, plataformas cloud, entornos de desarrollo, sistemas de CI/CD y arquitecturas que utilizan aplicaciones contenerizadas.

**¿Por qué me afecta?**  
Una configuración insegura puede permitir que un atacante escape del aislamiento, acceda a recursos del host o comprometa otros contenedores.

**¿Cómo se soluciona?**  
Utilizando imágenes confiables y actualizadas, ejecutando procesos con mínimos privilegios, limitando capacidades y recursos, y monitoreando la actividad de los contenedores.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar una vulnerabilidad de la aplicación o del runtime para comprometer el contenedor y buscar acceso a otros recursos del entorno.

## Docker

**¿Qué es?**  
Docker es una plataforma utilizada para crear, ejecutar y administrar aplicaciones empaquetadas como contenedores.

**¿Dónde lo encuentro?**  
En estaciones de desarrollo, servidores, pipelines de CI/CD, laboratorios y entornos cloud que utilizan contenedores.

**¿Por qué me afecta?**  
Una configuración insegura del daemon, imágenes vulnerables o contenedores con privilegios excesivos pueden aumentar el impacto de un compromiso.

**¿Cómo se soluciona?**  
Protegiendo el acceso al daemon, utilizando imágenes confiables, escaneando vulnerabilidades, aplicando mínimo privilegio y manteniendo Docker actualizado.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede abusar de un daemon Docker expuesto, una imagen comprometida o un contenedor privilegiado para ejecutar código y acceder a recursos adicionales.

## Kubernetes

**¿Qué es?**  
Kubernetes es una plataforma de orquestación que automatiza el despliegue, escalado y administración de aplicaciones contenerizadas.

**¿Dónde lo encuentro?**  
En clusters empresariales, entornos cloud, centros de datos y plataformas utilizadas para ejecutar aplicaciones distribuidas.

**¿Por qué me afecta?**  
Una configuración insegura del cluster, API, permisos o workloads puede permitir que un atacante controle recursos o se desplace dentro del entorno.

**¿Cómo se soluciona?**  
Aplicando RBAC y mínimo privilegio, protegiendo el API Server, utilizando políticas de red, gestionando secretos de forma segura y manteniendo los componentes actualizados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer una aplicación o cuenta con permisos excesivos y utilizarla para acceder a otros recursos, desplegar workloads maliciosos o intentar comprometer el cluster.

## Image

**¿Qué es?**  
Una Image es un paquete inmutable que contiene el sistema de archivos, dependencias y configuración necesarios para crear un contenedor.

**¿Dónde lo encuentro?**  
En estaciones de desarrollo, servidores, pipelines de CI/CD y registros de imágenes utilizados para almacenar y distribuir aplicaciones contenerizadas.

**¿Por qué me afecta?**  
Una imagen vulnerable o maliciosa puede introducir malware, vulnerabilidades o configuraciones inseguras en todos los contenedores creados a partir de ella.

**¿Cómo se soluciona?**  
Utilizando imágenes confiables, manteniéndolas actualizadas, escaneándolas antes del despliegue y evitando incluir secretos dentro de ellas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede introducir una imagen maliciosa en la cadena de suministro o explotar vulnerabilidades presentes en una imagen utilizada por la organización.

## Registry

**¿Qué es?**  
Un Registry es un repositorio utilizado para almacenar, administrar y distribuir imágenes de contenedores.

**¿Dónde lo encuentro?**  
En entornos de desarrollo, pipelines de CI/CD, infraestructuras cloud y plataformas que necesitan compartir imágenes entre diferentes sistemas.

**¿Por qué me afecta?**  
Un registry comprometido puede permitir modificar o reemplazar imágenes legítimas y distribuir código malicioso a múltiples entornos.

**¿Cómo se soluciona?**  
Protegiendo el acceso mediante autenticación y mínimo privilegio, escaneando imágenes, utilizando firmas cuando corresponda y monitoreando cambios en el repositorio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer una cuenta del registry, insertar una imagen maliciosa o modificar una imagen legítima para introducir código controlado por el atacante.

## Pod

**¿Qué es?**  
Un Pod es la unidad de ejecución más pequeña de Kubernetes y puede contener uno o varios contenedores que comparten determinados recursos, como red y almacenamiento.

**¿Dónde lo encuentro?**  
Dentro de clusters Kubernetes donde las aplicaciones contenerizadas se ejecutan y son administradas por el sistema de orquestación.

**¿Por qué me afecta?**  
Un Pod comprometido puede proporcionar al atacante acceso a aplicaciones, credenciales o recursos disponibles para los contenedores que contiene.

**¿Cómo se soluciona?**  
Aplicando Security Contexts, mínimo privilegio, políticas de red, límites de recursos y evitando contenedores privilegiados o configuraciones innecesariamente permisivas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer una aplicación dentro de un Pod y utilizar los permisos o recursos disponibles para intentar acceder a otros componentes del cluster.

## Cluster

**¿Qué es?**  
Un Cluster es un conjunto de nodos que trabajan conjuntamente para ejecutar y administrar cargas de trabajo, como ocurre en Kubernetes.

**¿Dónde lo encuentro?**  
En infraestructuras cloud, centros de datos y plataformas que ejecutan aplicaciones distribuidas mediante Kubernetes.

**¿Por qué me afecta?**  
El compromiso de componentes centrales del cluster puede afectar numerosas aplicaciones y recursos simultáneamente.

**¿Cómo se soluciona?**  
Protegiendo el plano de control, aplicando RBAC, segmentación de red, mínimo privilegio, actualizaciones y monitoreo de eventos del cluster.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales o permisos comprometidos para acceder al cluster, desplegar cargas maliciosas o manipular recursos existentes.

## Namespace

**¿Qué es?**  
Un Namespace es un mecanismo de Kubernetes utilizado para separar y organizar recursos dentro de un mismo cluster.

**¿Dónde lo encuentro?**  
En clusters Kubernetes donde diferentes aplicaciones, equipos o entornos necesitan administrar recursos de forma separada.

**¿Por qué me afecta?**  
Una configuración incorrecta de permisos o políticas entre namespaces puede permitir que una cuenta o workload acceda a recursos que deberían estar aislados.

**¿Cómo se soluciona?**  
Aplicando RBAC, políticas de red, separación lógica de recursos y controles de acceso específicos para cada namespace.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar permisos excesivos para consultar, modificar o crear recursos en otros namespaces y ampliar su acceso dentro del cluster.

## Service Account

**¿Qué es?**  
Una Service Account es una identidad utilizada por aplicaciones o workloads para autenticarse y acceder a recursos dentro de un sistema, como Kubernetes.

**¿Dónde lo encuentro?**  
En clusters Kubernetes y otros entornos donde aplicaciones necesitan identidades propias para interactuar con servicios o APIs.

**¿Por qué me afecta?**  
Una Service Account con permisos excesivos o comprometida puede permitir a un atacante realizar acciones privilegiadas dentro del entorno.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio mediante RBAC, evitando permisos innecesarios, protegiendo los tokens y revisando periódicamente las identidades utilizadas por los workloads.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede robar o abusar de las credenciales asociadas con una Service Account comprometida para acceder a recursos según los permisos asignados.

## Secret

**¿Qué es?**  
Un Secret es un recurso utilizado para almacenar información sensible, como contraseñas, tokens, claves o certificados necesarios para aplicaciones y servicios.

**¿Dónde lo encuentro?**  
En Kubernetes y otras plataformas donde las aplicaciones necesitan acceder a credenciales o información sensible durante su ejecución.

**¿Por qué me afecta?**  
Una exposición de Secrets puede proporcionar a un atacante credenciales válidas para acceder a bases de datos, APIs, servicios cloud u otros recursos.

**¿Cómo se soluciona?**  
Limitando el acceso mediante mínimo privilegio, protegiendo el almacenamiento de secretos, rotando credenciales y evitando incluir secretos directamente en imágenes o código.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar Secrets expuestos en configuraciones, variables, workloads o repositorios para obtener credenciales y utilizarlas contra otros servicios.
