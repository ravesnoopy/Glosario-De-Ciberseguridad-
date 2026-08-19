
## Firewall Blocking

**¿Qué es?**  
Firewall Blocking es una medida que impide conexiones de red que coinciden con reglas definidas por un firewall.

**¿Dónde lo encuentro?**  
En firewalls de red, firewalls de host, dispositivos de seguridad y servicios cloud que controlan el tráfico entrante o saliente.

**¿Por qué me afecta?**  
Permite impedir comunicaciones no autorizadas y reducir la exposición de sistemas frente a conexiones maliciosas.

**¿Cómo se soluciona?**  
Definiendo reglas basadas en el principio de mínimo privilegio, revisándolas periódicamente y registrando el tráfico bloqueado para su análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar utilizar puertos, protocolos o rutas permitidas para evadir las reglas del firewall y establecer comunicación con sistemas comprometidos.

## IP Blocking

**¿Qué es?**  
IP Blocking es una medida que impide conexiones desde o hacia una dirección IP específica identificada como no autorizada o maliciosa.

**¿Dónde lo encuentro?**  
En firewalls, sistemas de prevención de intrusiones, WAF, routers, servicios cloud y controles de seguridad de endpoints.

**¿Por qué me afecta?**  
Puede impedir rápidamente comunicaciones con infraestructura asociada con un atacante, aunque una IP por sí sola no siempre representa una identidad permanente.

**¿Cómo se soluciona?**  
Bloqueando las IP relevantes, validando la inteligencia que las identifica como maliciosas y revisando periódicamente las reglas para evitar bloqueos innecesarios.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cambiar de dirección IP, utilizar infraestructura comprometida o emplear servicios intermediarios para evitar el bloqueo.

## Domain Blocking

**¿Qué es?**  
Domain Blocking es una medida que impide el acceso o comunicación con dominios identificados como maliciosos, sospechosos o no autorizados.

**¿Dónde lo encuentro?**  
En DNS, firewalls, proxies, sistemas de seguridad de correo, navegadores administrados y soluciones de seguridad de endpoints.

**¿Por qué me afecta?**  
Puede impedir que usuarios o sistemas se comuniquen con sitios utilizados para phishing, malware, Command and Control u otras actividades maliciosas.

**¿Cómo se soluciona?**  
Bloqueando dominios maliciosos mediante controles de DNS, proxy o seguridad de endpoints y manteniendo actualizadas las listas de inteligencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede registrar nuevos dominios, utilizar dominios comprometidos o modificar su infraestructura para evadir los bloqueos existentes.

## Hash Blocking

**¿Qué es?**  
Hash Blocking es una medida que bloquea archivos o programas cuyo hash coincide con un valor identificado como malicioso.

**¿Dónde lo encuentro?**  
En antivirus, EDR, sistemas de prevención de malware y plataformas de seguridad que permiten crear indicadores basados en hashes.

**¿Por qué me afecta?**  
Permite impedir la ejecución o distribución de archivos conocidos como maliciosos y puede ser útil durante la respuesta a incidentes.

**¿Cómo se soluciona?**  
Identificando hashes maliciosos confiables, aplicando reglas de bloqueo y complementando este control con análisis de comportamiento y otras técnicas de detección.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar un archivo malicioso para generar un hash diferente y evitar un bloqueo basado únicamente en su valor hash.

## Quarantine

**¿Qué es?**  
Quarantine es una medida de seguridad que aísla un archivo, dispositivo, cuenta o recurso sospechoso para impedir que continúe interactuando normalmente con el entorno.

**¿Dónde lo encuentro?**  
En soluciones EDR, antivirus, sistemas de correo, plataformas de respuesta a incidentes y controles de seguridad de endpoints.

**¿Por qué me afecta?**  
Permite contener una amenaza mientras se determina si es maliciosa, reduciendo la posibilidad de que continúe propagándose o causando daños.

**¿Cómo se soluciona?**  
Aislando el elemento afectado, analizando la evidencia, determinando su naturaleza y eliminándolo o restaurándolo según corresponda.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar detectar o evadir mecanismos de cuarentena, modificar su comportamiento o eliminar indicadores antes de que el sistema lo aísle.
