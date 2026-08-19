
## Tactic Mapping

**¿Qué es?**  
Proceso de relacionar una actividad, comportamiento o hallazgo de seguridad con una táctica que representa el objetivo general de un atacante.

**¿Dónde lo encuentro?**  
En análisis de incidentes, Threat Intelligence, Threat Hunting y documentación basada en MITRE ATT&CK.

**¿Por qué me afecta?**  
Permite entender qué objetivos persigue un atacante y detectar posibles etapas posteriores de una intrusión.

**¿Cómo se soluciona?**  
Mapear las actividades observadas a las tácticas correspondientes y utilizar ese contexto para evaluar cobertura y posibles brechas de detección.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría avanzar entre diferentes tácticas de ataque sin generar suficiente actividad detectable para evitar que su operación sea identificada.


## Technique Mapping

**¿Qué es?**  
Proceso de relacionar comportamientos o acciones observadas durante una investigación con técnicas específicas utilizadas por los atacantes.

**¿Dónde lo encuentro?**  
En investigaciones de incidentes, Threat Hunting, Threat Intelligence, detección y análisis basado en MITRE ATT&CK.

**¿Por qué me afecta?**  
Permite describir técnicamente cómo se ejecutó una actividad maliciosa y evaluar si existen controles capaces de detectarla.

**¿Cómo se soluciona?**  
Analizar la evidencia disponible, identificar la técnica correspondiente y relacionarla con las detecciones y controles existentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría cambiar herramientas o procedimientos mientras mantiene una técnica similar, intentando aprovechar brechas en la cobertura de detección.


## ATT&CK Navigator

**¿Qué es?**  
Herramienta que permite visualizar y documentar técnicas y tácticas de MITRE ATT&CK para analizar comportamientos, cobertura de detección y posibles brechas.

**¿Dónde lo encuentro?**  
En análisis de amenazas, investigaciones, Threat Hunting, planificación de detecciones y evaluación de cobertura de seguridad.

**¿Por qué me afecta?**  
Ayuda a visualizar qué técnicas están cubiertas por los controles actuales y dónde existen áreas con poca o ninguna detección.

**¿Cómo se soluciona?**  
Mantener los mapas actualizados con técnicas relevantes, relacionarlos con detecciones existentes y priorizar las brechas de mayor riesgo.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría utilizar técnicas que presenten poca cobertura de detección para reducir la probabilidad de ser identificado durante su actividad.


## Detection Engineering

**¿Qué es?**  
Disciplina enfocada en diseñar, implementar, probar y mantener detecciones capaces de identificar actividades sospechosas o maliciosas.

**¿Dónde lo encuentro?**  
En SOC, SIEM, EDR, plataformas de monitoreo y equipos dedicados al desarrollo de capacidades de detección.

**¿Por qué me afecta?**  
Una detección deficiente puede generar demasiados falsos positivos o no identificar comportamientos importantes durante un ataque.

**¿Cómo se soluciona?**  
Diseñar detecciones basadas en amenazas y comportamiento, probarlas con datos reales, medir su eficacia y ajustarlas continuamente.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría modificar sus acciones para evitar las condiciones que generan alertas o aprovechar detecciones demasiado específicas y fáciles de evadir.


## Threat Hunting

**¿Qué es?**  
Proceso proactivo de buscar amenazas o comportamientos sospechosos dentro de un entorno sin depender exclusivamente de alertas generadas automáticamente.

**¿Dónde lo encuentro?**  
En SOC, equipos de Threat Intelligence, EDR, SIEM, análisis de logs y operaciones de detección y respuesta.

**¿Por qué me afecta?**  
Puede descubrir actividad maliciosa que no fue detectada por las reglas o herramientas existentes.

**¿Cómo se soluciona?**  
Crear hipótesis de búsqueda, analizar telemetría relevante, investigar comportamientos y convertir los hallazgos en nuevas detecciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría mantener sus acciones dentro de comportamientos habituales para dificultar su identificación mediante búsquedas proactivas.


## Behavioral Detection

**¿Qué es?**  
Método de detección que identifica amenazas mediante comportamientos y secuencias de actividad sospechosas en lugar de depender únicamente de indicadores conocidos.

**¿Dónde lo encuentro?**  
En EDR, SIEM, sistemas de análisis de comportamiento, monitoreo de endpoints y plataformas de seguridad.

**¿Por qué me afecta?**  
Puede detectar amenazas nuevas o modificadas incluso cuando sus archivos, hashes, dominios u otros indicadores no son conocidos.

**¿Cómo se soluciona?**  
Definir comportamientos esperados, identificar desviaciones relevantes y crear detecciones basadas en contexto y secuencias de acciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría imitar comportamientos legítimos, reducir acciones sospechosas o distribuirlas en el tiempo para evitar generar patrones claramente maliciosos.
