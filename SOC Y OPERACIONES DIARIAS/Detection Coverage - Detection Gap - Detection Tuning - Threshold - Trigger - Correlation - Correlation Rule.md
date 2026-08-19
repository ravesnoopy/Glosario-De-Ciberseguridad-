
## Detection Coverage

**¿Qué es?**  
Detection Coverage es el grado en que las reglas y controles de detección de una organización pueden identificar técnicas, comportamientos y actividades relevantes de una amenaza.

**¿Dónde lo encuentro?**  
En programas de detección, SIEM, EDR, plataformas de threat hunting y evaluaciones de cobertura frente a marcos como MITRE ATT&CK.

**¿Por qué me afecta?**  
Una cobertura insuficiente puede permitir que determinadas fases o técnicas de un ataque ocurran sin generar alertas.

**¿Cómo se soluciona?**  
Evaluando las técnicas relevantes, identificando qué comportamientos pueden detectarse y desarrollando o mejorando reglas para cubrir las brechas existentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar técnicas que no estén cubiertas por las detecciones disponibles para avanzar dentro del entorno sin generar alertas.

## Detection Gap

**¿Qué es?**  
Detection Gap es una deficiencia en la capacidad de una organización para detectar una actividad, técnica o etapa específica de un ataque.

**¿Dónde lo encuentro?**  
En evaluaciones de seguridad, revisiones de reglas SIEM, ejercicios de Threat Hunting y análisis de cobertura de detecciones.

**¿Por qué me afecta?**  
Una brecha de detección puede permitir que una actividad maliciosa permanezca sin identificar durante una parte importante del ataque.

**¿Cómo se soluciona?**  
Identificando qué datos o reglas faltan, mejorando la telemetría y creando o ajustando detecciones para cubrir la actividad no identificada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar técnicas que presenten una Detection Gap para reducir la probabilidad de ser descubierto.

## Detection Tuning

**¿Qué es?**  
Detection Tuning es el proceso de ajustar reglas y parámetros de detección para mejorar su precisión y reducir falsos positivos sin perder cobertura relevante.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, sistemas de monitoreo y procesos de mantenimiento de reglas de detección.

**¿Por qué me afecta?**  
Una detección mal ajustada puede generar demasiadas alertas irrelevantes o, al contrario, ser demasiado restrictiva y omitir amenazas reales.

**¿Cómo se soluciona?**  
Revisando alertas históricas, ajustando condiciones y excepciones, y validando que los cambios mantengan la capacidad de detectar actividad maliciosa.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar actividad que se parezca a comportamientos legítimos para aprovechar reglas demasiado permisivas o provocar falsos positivos.

## Threshold

**¿Qué es?**  
Threshold es un límite o cantidad definida que, al alcanzarse o superarse, puede provocar una alerta o una acción de detección.

**¿Dónde lo encuentro?**  
En reglas SIEM, sistemas de detección, monitoreo de autenticaciones, análisis de comportamiento y controles de seguridad.

**¿Por qué me afecta?**  
Un Threshold demasiado alto puede permitir que una actividad maliciosa pase desapercibida, mientras que uno demasiado bajo puede generar demasiados falsos positivos.

**¿Cómo se soluciona?**  
Definiendo valores basados en el comportamiento normal del entorno y ajustándolos mediante análisis de alertas y resultados de investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede mantener su actividad por debajo del umbral configurado para evitar que se genere una alerta.

## Trigger

**¿Qué es?**  
Trigger es la condición o evento que provoca que una regla de detección, alerta o acción automatizada se active.

**¿Dónde lo encuentro?**  
En SIEM, EDR, SOAR, sistemas de monitoreo y reglas de seguridad automatizadas.

**¿Por qué me afecta?**  
Un Trigger correctamente definido permite detectar comportamientos específicos y responder rápidamente ante actividades sospechosas.

**¿Cómo se soluciona?**  
Definiendo condiciones relevantes, probándolas con datos reales y revisándolas periódicamente para mantener su efectividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar su comportamiento para evitar las condiciones que activan los triggers de las reglas de detección.

## Correlation

**¿Qué es?**  
Correlation es el proceso de relacionar múltiples eventos o datos para identificar una actividad o patrón que podría no ser evidente al analizar cada evento individualmente.

**¿Dónde lo encuentro?**  
En SIEM, plataformas de detección, sistemas de monitoreo y herramientas de análisis de seguridad.

**¿Por qué me afecta?**  
Permite conectar eventos de diferentes fuentes y descubrir cadenas de actividad que podrían indicar un ataque.

**¿Cómo se soluciona?**  
Integrando fuentes relevantes, sincronizando correctamente los eventos y definiendo relaciones basadas en tiempo, identidad, host, IP u otros atributos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede distribuir sus actividades entre diferentes sistemas, cuentas o períodos de tiempo para dificultar su correlación.

## Correlation Rule

**¿Qué es?**  
Correlation Rule es una regla que define condiciones para relacionar múltiples eventos y generar una alerta cuando el conjunto de eventos coincide con un patrón determinado.

**¿Dónde lo encuentro?**  
Principalmente en SIEM y plataformas de detección y monitoreo de seguridad.

**¿Por qué me afecta?**  
Permite detectar secuencias de eventos que individualmente pueden parecer normales pero que, combinadas, pueden indicar un ataque.

**¿Cómo se soluciona?**  
Diseñando reglas basadas en comportamientos relevantes, probándolas con datos reales y ajustándolas para mantener una buena relación entre cobertura y falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar la secuencia, frecuencia o características de sus acciones para evitar que coincidan con las condiciones definidas en una Correlation Rule.
