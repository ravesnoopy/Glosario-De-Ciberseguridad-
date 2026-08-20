
## Alert

**¿Qué es?**  
Alert es una notificación generada cuando una herramienta de seguridad identifica una condición o actividad que requiere revisión.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, firewalls, sistemas de monitoreo y plataformas de gestión de seguridad.

**¿Por qué me afecta?**  
Una alerta puede ser la primera señal de una actividad maliciosa y ayudar a iniciar una investigación antes de que aumente el impacto.

**¿Cómo se soluciona?**  
Validando la alerta, evaluando su contexto, determinando su severidad y aplicando las acciones de respuesta correspondientes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar grandes cantidades de actividad para producir ruido y dificultar que los analistas identifiquen alertas realmente importantes.

## Detection

**¿Qué es?**  
Detection es el proceso o capacidad de identificar actividades, eventos o comportamientos que pueden indicar una amenaza de seguridad.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, NDR, herramientas de Threat Hunting y otros controles de seguridad.

**¿Por qué me afecta?**  
Una detección efectiva permite identificar amenazas y comportamientos sospechosos antes de que provoquen un impacto mayor.

**¿Cómo se soluciona?**  
Mejorando la telemetría, desarrollando reglas adecuadas, validando resultados y revisando periódicamente la cobertura de detección.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentará modificar su comportamiento, utilizar herramientas legítimas o reducir sus indicadores para evitar ser detectado.

## Rule

**¿Qué es?**  
Rule es una condición definida para identificar, clasificar o desencadenar una acción cuando determinados eventos o comportamientos ocurren.

**¿Dónde lo encuentro?**  
En SIEM, firewalls, IDS, EDR, sistemas de monitoreo y plataformas de automatización de seguridad.

**¿Por qué me afecta?**  
Las reglas permiten convertir eventos observados en decisiones, como generar una alerta, bloquear una conexión o iniciar una investigación.

**¿Cómo se soluciona?**  
Definiendo condiciones precisas, probándolas con datos reales y revisándolas para mantener un equilibrio entre cobertura y falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar sus acciones para evitar las condiciones específicas que activan las reglas de seguridad.

## Correlation

**¿Qué es?**  
Correlation es el proceso de relacionar múltiples eventos para identificar patrones que pueden revelar una actividad sospechosa.

**¿Dónde lo encuentro?**  
Principalmente en SIEM, sistemas de detección y plataformas de análisis de seguridad.

**¿Por qué me afecta?**  
Permite detectar cadenas de actividad que pueden parecer normales cuando se observan individualmente, pero que resultan sospechosas al analizarse en conjunto.

**¿Cómo se soluciona?**  
Integrando fuentes relevantes y correlacionando eventos mediante atributos como tiempo, usuario, host, IP y comportamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede distribuir sus acciones entre diferentes cuentas, sistemas o períodos de tiempo para dificultar la correlación.

## Query

**¿Qué es?**  
Query es una consulta utilizada para buscar, filtrar o analizar información dentro de un conjunto de datos, como registros de seguridad.

**¿Dónde lo encuentro?**  
En SIEM, plataformas de Threat Hunting, bases de datos de logs, EDR y herramientas de análisis.

**¿Por qué me afecta?**  
Permite investigar eventos específicos, buscar indicadores y encontrar patrones que pueden revelar actividad maliciosa.

**¿Cómo se soluciona?**  
Construyendo consultas precisas, utilizando los campos disponibles y validando los resultados para evitar interpretaciones incorrectas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar indicadores o utilizar variaciones de sus técnicas para evitar coincidir con consultas demasiado específicas.

## Baseline

**¿Qué es?**  
Baseline es una referencia del comportamiento normal esperado para un usuario, sistema, aplicación o red.

**¿Dónde lo encuentro?**  
En SIEM, EDR, monitoreo de redes, análisis de comportamiento y procesos de seguridad.

**¿Por qué me afecta?**  
Permite comparar la actividad actual con el comportamiento esperado e identificar desviaciones potencialmente sospechosas.

**¿Cómo se soluciona?**  
Estableciendo referencias basadas en actividad legítima y actualizándolas cuando cambian los sistemas o patrones normales del entorno.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede mantener sus acciones dentro de patrones similares al comportamiento legítimo para evitar generar desviaciones evidentes.

## Anomaly

**¿Qué es?**  
Anomaly es una actividad o evento que se desvía del comportamiento considerado normal para un sistema, usuario o entorno.

**¿Dónde lo encuentro?**  
En SIEM, EDR, NDR, herramientas de análisis de comportamiento y sistemas de detección de anomalías.

**¿Por qué me afecta?**  
Una anomalía puede ser una señal temprana de compromiso, abuso de credenciales o actividad maliciosa, aunque no necesariamente represente un ataque.

**¿Cómo se soluciona?**  
Analizando el contexto de la anomalía, comparándola con el baseline y determinando si corresponde a actividad legítima o requiere investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede mantener una actividad gradual y similar al comportamiento normal para reducir las anomalías que genera y dificultar su detección.
