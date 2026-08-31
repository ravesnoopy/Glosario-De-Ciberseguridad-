## API Security

**¿Qué es?**  
API Security es el conjunto de prácticas y controles destinados a proteger las APIs contra accesos no autorizados, abuso y explotación de vulnerabilidades.

**¿Dónde lo encuentro?**  
En APIs web, aplicaciones móviles, microservicios, servicios cloud y sistemas que intercambian información entre aplicaciones.

**¿Por qué me afecta?**  
Una API vulnerable puede permitir acceso no autorizado, exposición de datos, modificación de recursos o abuso de funciones.

**¿Cómo se soluciona?**  
Aplicando autenticación, autorización, validación de entradas, cifrado, rate limiting y monitoreo de las solicitudes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede descubrir endpoints, manipular parámetros o explotar controles de seguridad deficientes para acceder o modificar información.

## Access Control

**¿Qué es?**  
Access Control es el conjunto de mecanismos que determina qué usuarios, procesos o sistemas pueden acceder a determinados recursos y qué acciones pueden realizar.

**¿Dónde lo encuentro?**  
En sistemas operativos, aplicaciones, APIs, bases de datos, redes y servicios cloud.

**¿Por qué me afecta?**  
Un control de acceso incorrecto puede permitir que un usuario acceda a información o funciones que no debería utilizar.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, autenticación adecuada, autorización basada en roles o atributos y revisiones periódicas de permisos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar permisos excesivos o fallos de autorización para acceder a recursos restringidos.

## Input Validation

**¿Qué es?**  
Input Validation es el proceso de verificar que los datos recibidos por una aplicación cumplen con el formato, tipo, longitud y valores esperados.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, formularios, scripts y servicios que reciben datos externos.

**¿Por qué me afecta?**  
Una validación insuficiente puede permitir entradas maliciosas que provoquen vulnerabilidades como inyección o manipulación de parámetros.

**¿Cómo se soluciona?**  
Validando las entradas en el servidor mediante tipos de datos, límites de longitud, formatos esperados y listas de valores permitidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enviar datos especialmente construidos para explotar la forma en que una aplicación procesa entradas no confiables.

## Secure Configuration

**¿Qué es?**  
Secure Configuration es la configuración de sistemas, aplicaciones y dispositivos utilizando parámetros que reducen su exposición y riesgo de seguridad.

**¿Dónde lo encuentro?**  
En servidores, endpoints, aplicaciones, dispositivos de red, bases de datos y servicios cloud.

**¿Por qué me afecta?**  
Las configuraciones inseguras pueden habilitar servicios innecesarios, permisos excesivos, credenciales predeterminadas o funcionalidades que aumentan la superficie de ataque.

**¿Cómo se soluciona?**  
Deshabilitando servicios innecesarios, eliminando configuraciones predeterminadas inseguras, restringiendo permisos y aplicando configuraciones verificadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar configuraciones débiles, servicios expuestos o credenciales predeterminadas para obtener acceso o ampliar su control.

## Hardening

**¿Qué es?**  
Hardening es el proceso de reducir la superficie de ataque de un sistema mediante la eliminación o restricción de componentes, servicios, permisos y configuraciones innecesarias.

**¿Dónde lo encuentro?**  
En sistemas operativos, servidores, endpoints, aplicaciones, dispositivos de red y entornos cloud.

**¿Por qué me afecta?**  
Un sistema sin hardening puede exponer más servicios y funcionalidades que un atacante puede identificar y explotar.

**¿Cómo se soluciona?**  
Deshabilitando componentes innecesarios, limitando privilegios, aplicando actualizaciones y configurando los servicios de forma segura.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar sistemas que no fueron endurecidos y aprovechar servicios, permisos o configuraciones débiles.

## Security Baseline

**¿Qué es?**  
Security Baseline es un conjunto de configuraciones y controles mínimos de seguridad utilizados como referencia para sistemas, dispositivos o aplicaciones.

**¿Dónde lo encuentro?**  
En organizaciones, sistemas operativos, infraestructura cloud, estándares de configuración y procesos de gestión de seguridad.

**¿Por qué me afecta?**  
Permite establecer un nivel mínimo de seguridad y detectar sistemas cuya configuración se desvía de los controles establecidos.

**¿Cómo se soluciona?**  
Definiendo una baseline adecuada, aplicándola de forma consistente y verificando periódicamente su cumplimiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar sistemas que se encuentren por debajo de la Security Baseline para aprovechar configuraciones débiles o controles ausentes.
