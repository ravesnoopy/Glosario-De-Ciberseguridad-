
## API

**¿Qué es?**  
API (Application Programming Interface) es un conjunto de reglas y mecanismos que permite que diferentes aplicaciones o sistemas se comuniquen e intercambien datos o funciones.

**¿Dónde lo encuentro?**  
En aplicaciones web, aplicaciones móviles, servicios internos, plataformas cloud y sistemas que necesitan comunicarse con otros componentes.

**¿Por qué me afecta?**  
Una API mal diseñada o protegida puede exponer información, funciones administrativas o recursos internos a usuarios no autorizados.

**¿Cómo se soluciona?**  
Implementando autenticación y autorización adecuadas, validando entradas, limitando solicitudes, protegiendo datos sensibles y monitoreando el tráfico de la API.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede analizar los endpoints disponibles y enviar solicitudes manipuladas para acceder a información, abusar de funciones o explotar vulnerabilidades.

## REST API

**¿Qué es?**  
REST API es una API que sigue los principios de REST (Representational State Transfer) para permitir la comunicación entre sistemas mediante operaciones sobre recursos, normalmente utilizando HTTP.

**¿Dónde lo encuentro?**  
En aplicaciones web, aplicaciones móviles, servicios cloud y arquitecturas de microservicios que utilizan endpoints HTTP para intercambiar datos, frecuentemente en formato JSON.

**¿Por qué me afecta?**  
Una REST API expuesta puede convertirse en una superficie de ataque si existen fallos de autenticación, autorización, validación de entradas o controles de acceso.

**¿Cómo se soluciona?**  
Aplicando autenticación y autorización robustas, validación de entradas, HTTPS, límites de solicitudes, controles de acceso y monitoreo de los endpoints.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enumerar endpoints y manipular parámetros o solicitudes para acceder a recursos no autorizados, abusar de funciones o explotar vulnerabilidades.

## SOAP

**¿Qué es?**  
SOAP (Simple Object Access Protocol) es un protocolo basado en XML utilizado para intercambiar mensajes estructurados entre sistemas, especialmente en servicios empresariales.

**¿Dónde lo encuentro?**  
En aplicaciones empresariales, sistemas legacy, servicios financieros, integraciones entre organizaciones y aplicaciones que utilizan servicios web basados en XML.

**¿Por qué me afecta?**  
Una implementación SOAP insegura puede exponer información sensible o ser vulnerable a problemas como XML External Entity (XXE), inyección XML y ataques de denegación de servicio.

**¿Cómo se soluciona?**  
Validando y restringiendo el procesamiento de XML, deshabilitando funcionalidades XML innecesarias, utilizando autenticación y autorización adecuadas y protegiendo la comunicación mediante HTTPS.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede enviar mensajes XML manipulados para explotar el procesamiento del servicio, provocar consumo excesivo de recursos o intentar acceder a información no autorizada.
