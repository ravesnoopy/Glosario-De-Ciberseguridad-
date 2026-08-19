
## DNS Resolution

**¿Qué es?**  
Proceso mediante el cual un nombre de dominio se traduce a la información necesaria para localizar un recurso o servicio de red, como una dirección IP.

**¿Dónde lo encuentro?**  
En navegadores, sistemas operativos, aplicaciones, servidores DNS y prácticamente cualquier entorno que utilice nombres de dominio.

**¿Por qué me afecta?**  
Las resoluciones DNS permiten identificar comunicaciones legítimas y también pueden revelar conexiones hacia dominios sospechosos o infraestructura maliciosa.

**¿Cómo se soluciona?**  
Utilizar servidores DNS confiables, monitorear consultas, aplicar filtrado y analizar dominios sospechosos según su contexto.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría utilizar DNS para localizar infraestructura maliciosa, establecer comunicaciones de C2 o realizar reconocimiento del entorno.


## A Record

**¿Qué es?**  
Registro DNS que asocia un nombre de dominio o host con una dirección IPv4.

**¿Dónde lo encuentro?**  
En zonas DNS de dominios, servidores DNS y configuraciones de infraestructura de red.

**¿Por qué me afecta?**  
Una consulta A puede revelar qué dirección IPv4 está asociada con un servicio o infraestructura determinada.

**¿Cómo se soluciona?**  
Mantener registros DNS correctos, eliminar entradas innecesarias y proteger la administración de las zonas DNS.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría consultar registros A para identificar servidores asociados con dominios y utilizarlos durante actividades de reconocimiento.


## AAAA Record

**¿Qué es?**  
Registro DNS que asocia un nombre de dominio o host con una dirección IPv6.

**¿Dónde lo encuentro?**  
En zonas DNS y configuraciones de servicios que utilizan conectividad IPv6.

**¿Por qué me afecta?**  
Una configuración IPv6 olvidada o incorrecta puede proporcionar una ruta de acceso que no esté cubierta por los controles aplicados a IPv4.

**¿Cómo se soluciona?**  
Gestionar IPv6 de forma coherente con IPv4, proteger los registros DNS y aplicar controles de seguridad también sobre el tráfico IPv6.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría buscar servicios accesibles mediante IPv6 que no estén correctamente protegidos o monitoreados.


## CNAME

**¿Qué es?**  
Registro DNS que crea un alias de un nombre de dominio hacia otro nombre de dominio.

**¿Dónde lo encuentro?**  
En zonas DNS de sitios web, servicios cloud, aplicaciones y otros servicios que utilizan alias de nombres.

**¿Por qué me afecta?**  
Una configuración incorrecta o un alias que apunte a un recurso abandonado puede generar riesgos de seguridad.

**¿Cómo se soluciona?**  
Revisar periódicamente los registros CNAME, eliminar referencias innecesarias y verificar que los destinos sigan bajo control de la organización.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar aprovechar un alias que apunte a un recurso abandonado o mal configurado para obtener control sobre el servicio asociado.


## MX Record

**¿Qué es?**  
Registro DNS que indica qué servidores están autorizados a recibir correo electrónico para un dominio.

**¿Dónde lo encuentro?**  
En las zonas DNS de dominios que utilizan servicios de correo electrónico.

**¿Por qué me afecta?**  
Una configuración incorrecta puede afectar la entrega del correo o facilitar ataques relacionados con suplantación y abuso del dominio.

**¿Cómo se soluciona?**  
Mantener correctamente configurados los servidores de correo y complementar la protección con mecanismos de autenticación y políticas de correo.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría investigar los registros MX para identificar la infraestructura de correo y utilizar esa información durante campañas de phishing o reconocimiento.


## TXT Record

**¿Qué es?**  
Registro DNS utilizado para almacenar información textual asociada con un dominio, incluyendo configuraciones y mecanismos de validación.

**¿Dónde lo encuentro?**  
En zonas DNS de dominios y servicios que requieren publicar información de configuración o verificación.

**¿Por qué me afecta?**  
Puede contener información relevante sobre servicios, autenticación de correo y verificaciones de propiedad del dominio.

**¿Cómo se soluciona?**  
Revisar periódicamente su contenido, evitar publicar información innecesaria y mantener configuraciones de autenticación correctamente administradas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría consultar registros TXT para recopilar información sobre servicios, configuraciones o mecanismos utilizados por una organización.


## PTR Record

**¿Qué es?**  
Registro DNS utilizado para realizar una resolución inversa, asociando una dirección IP con un nombre de dominio.

**¿Dónde lo encuentro?**  
En DNS inverso, servidores de nombres y servicios que necesitan identificar nombres asociados con direcciones IP.

**¿Por qué me afecta?**  
Puede proporcionar información adicional sobre la infraestructura asociada con una dirección IP y ayudar a validar la identidad de determinados servicios.

**¿Cómo se soluciona?**  
Mantener registros PTR coherentes y controlar qué información de infraestructura se expone públicamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría consultar registros PTR para obtener nombres asociados con direcciones IP y ampliar el reconocimiento de la infraestructura.


## DHCP Lease

**¿Qué es?**  
Asignación temporal mediante la cual un servidor DHCP proporciona a un dispositivo una dirección IP y otros parámetros de configuración durante un periodo determinado.

**¿Dónde lo encuentro?**  
En servidores DHCP, routers, dispositivos de red y registros de configuración de clientes.

**¿Por qué me afecta?**  
Los leases permiten relacionar direcciones IP con dispositivos y periodos de uso, proporcionando información útil para administración y análisis de incidentes.

**¿Cómo se soluciona?**  
Mantener registros DHCP adecuados, proteger el servidor y correlacionar los leases con logs de autenticación y red.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar un DHCP comprometido o no autorizado para asignar configuraciones de red maliciosas o dificultar la identificación del dispositivo que utilizó una dirección IP.
