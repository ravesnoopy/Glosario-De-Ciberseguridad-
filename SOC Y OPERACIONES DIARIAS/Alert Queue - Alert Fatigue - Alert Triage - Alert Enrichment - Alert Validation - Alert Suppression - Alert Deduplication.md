
## Alert Queue

**¿Qué es?**  
Alert Queue es la cola donde se almacenan y organizan las alertas generadas por herramientas de seguridad antes de ser revisadas o procesadas por un analista.

**¿Dónde lo encuentro?**  
En SIEM, EDR, plataformas de monitoreo, sistemas de ticketing y consolas utilizadas por equipos SOC.

**¿Por qué me afecta?**  
Una cola saturada puede retrasar la revisión de alertas importantes y aumentar el riesgo de que un incidente real pase desapercibido.

**¿Cómo se soluciona?**  
Priorizando las alertas según riesgo, automatizando tareas repetitivas y estableciendo procedimientos claros de clasificación y escalamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar múltiples eventos o alertas de bajo valor para saturar la cola y dificultar que los analistas detecten actividades realmente maliciosas.

## Alert Fatigue

**¿Qué es?**  
Alert Fatigue es la disminución de la atención de los analistas causada por un volumen excesivo de alertas, especialmente cuando muchas son falsos positivos o de bajo riesgo.

**¿Dónde lo encuentro?**  
En equipos SOC que reciben grandes cantidades de alertas provenientes de SIEM, EDR, IDS, firewalls y otras herramientas.

**¿Por qué me afecta?**  
Puede provocar que un analista ignore, cierre rápidamente o pase por alto una alerta legítima entre muchas alertas poco relevantes.

**¿Cómo se soluciona?**  
Reduciendo falsos positivos, ajustando reglas, priorizando riesgos y automatizando el enriquecimiento y clasificación de alertas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar ruido mediante múltiples actividades benignas o de bajo impacto para aumentar el volumen de alertas y ocultar acciones maliciosas.

## Alert Triage

**¿Qué es?**  
Alert Triage es el proceso inicial de analizar y clasificar una alerta para determinar su prioridad, relevancia y posible impacto.

**¿Dónde lo encuentro?**  
En SOC, SIEM, EDR y procesos de respuesta a incidentes donde los analistas revisan alertas antes de realizar una investigación más profunda.

**¿Por qué me afecta?**  
Un triage incorrecto puede provocar que una amenaza real sea descartada o que recursos del SOC se utilicen en eventos de bajo riesgo.

**¿Cómo se soluciona?**  
Utilizando criterios consistentes de severidad, contexto del activo, comportamiento observado e indicadores de compromiso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar acciones que parezcan legítimas o de bajo riesgo para aumentar la probabilidad de que una alerta sea clasificada incorrectamente.

## Alert Enrichment

**¿Qué es?**  
Alert Enrichment es el proceso de agregar información contextual a una alerta para facilitar su análisis y determinar su riesgo.

**¿Dónde lo encuentro?**  
En SIEM, SOAR, plataformas de threat intelligence y flujos automatizados de investigación.

**¿Por qué me afecta?**  
El contexto adicional puede ayudar a determinar si una alerta corresponde a una actividad legítima, sospechosa o maliciosa.

**¿Cómo se soluciona?**  
Integrando información como reputación de IP, identidad del usuario, criticidad del activo, historial y threat intelligence.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar infraestructura con buena reputación o información aparentemente legítima para dificultar la interpretación del contexto asociado con una alerta.

## Alert Validation

**¿Qué es?**  
Alert Validation es el proceso de verificar si una alerta representa realmente una actividad sospechosa o un incidente de seguridad.

**¿Dónde lo encuentro?**  
En SOC, SIEM, EDR y procedimientos de análisis donde los analistas confirman o descartan alertas.

**¿Por qué me afecta?**  
Una validación incorrecta puede provocar que una amenaza real sea descartada como falso positivo o que se investiguen eventos que no representan riesgo.

**¿Cómo se soluciona?**  
Correlacionando la alerta con logs, contexto del usuario y activo, comportamiento histórico y otros indicadores disponibles.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede imitar comportamientos legítimos para dificultar que los analistas validen la actividad como maliciosa.

## Alert Suppression

**¿Qué es?**  
Alert Suppression es la práctica de evitar que determinadas alertas se generen o se presenten repetidamente cuando se cumplen condiciones definidas.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, sistemas de detección y plataformas de gestión de alertas.

**¿Por qué me afecta?**  
Una supresión demasiado amplia puede ocultar eventos relevantes y reducir la capacidad de detectar una amenaza.

**¿Cómo se soluciona?**  
Aplicando reglas de supresión específicas, documentadas y revisadas periódicamente para evitar ocultar señales importantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar generar eventos que coincidan con condiciones de supresión existentes para evitar que actividades maliciosas produzcan alertas.

## Alert Deduplication

**¿Qué es?**  
Alert Deduplication es el proceso de identificar y combinar alertas que representan el mismo evento o actividad para evitar análisis repetidos.

**¿Dónde lo encuentro?**  
En SIEM, plataformas SOC, sistemas de ticketing y herramientas de gestión de alertas.

**¿Por qué me afecta?**  
Reduce el volumen de alertas repetidas y permite que los analistas concentren su atención en incidentes distintos y relevantes.

**¿Cómo se soluciona?**  
Definiendo criterios adecuados para identificar alertas duplicadas sin combinar eventos que correspondan a actividades diferentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar eventos similares o repetitivos para intentar que actividades distintas sean agrupadas y dificultar la identificación de una cadena de ataque.
