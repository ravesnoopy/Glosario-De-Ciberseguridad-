
## False Positive

**¿Qué es?**  
False Positive es una alerta que inicialmente parece indicar una actividad maliciosa, pero después de analizarla se determina que corresponde a una actividad legítima.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, antivirus y otras herramientas que generan alertas de seguridad.

**¿Por qué me afecta?**  
Un volumen elevado de falsos positivos puede generar Alert Fatigue y hacer que los analistas pasen por alto amenazas reales.

**¿Cómo se soluciona?**  
Ajustando las reglas de detección, incorporando contexto y creando excepciones controladas para actividades legítimas conocidas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar actividad que produzca numerosos falsos positivos para crear ruido y dificultar la identificación de sus acciones maliciosas.

## True Positive

**¿Qué es?**  
True Positive es una alerta que identifica correctamente una actividad que realmente representa una amenaza o una condición de seguridad que requiere atención.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, antivirus y procesos de monitoreo y respuesta de seguridad.

**¿Por qué me afecta?**  
Representa una señal válida que puede indicar un ataque o compromiso y que requiere investigación y, cuando corresponda, respuesta.

**¿Cómo se soluciona?**  
Validando la alerta, determinando su alcance e impacto y aplicando las acciones de contención, erradicación y recuperación necesarias.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentará evitar generar señales que coincidan con las condiciones de detección para reducir la probabilidad de ser identificado.

## Triage

**¿Qué es?**  
Triage es el proceso inicial de revisar, validar y priorizar una alerta o evento para determinar su relevancia y los siguientes pasos de investigación.

**¿Dónde lo encuentro?**  
En SOC, SIEM, EDR, sistemas de gestión de alertas y procesos de Incident Response.

**¿Por qué me afecta?**  
Permite concentrar los recursos del equipo en las alertas con mayor probabilidad de representar una amenaza.

**¿Cómo se soluciona?**  
Aplicando criterios consistentes de severidad, contexto, criticidad del activo, identidad y comportamiento observado.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede diseñar sus acciones para parecer legítimas o de bajo riesgo y aumentar la probabilidad de que una alerta sea descartada durante el triage.

## Investigation

**¿Qué es?**  
Investigation es el proceso de analizar evidencia y eventos relacionados para determinar qué ocurrió, cómo ocurrió, qué sistemas fueron afectados y cuál fue el alcance de una actividad sospechosa.

**¿Dónde lo encuentro?**  
En SOC, DFIR, Threat Hunting, SIEM, EDR y procesos de respuesta a incidentes.

**¿Por qué me afecta?**  
Permite comprender el incidente, identificar sistemas comprometidos y obtener información necesaria para contener y remediar la amenaza.

**¿Cómo se soluciona?**  
Recopilando evidencia, construyendo una línea temporal, correlacionando eventos y documentando los hallazgos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede eliminar evidencia, modificar registros o utilizar técnicas que dificulten reconstruir sus acciones durante la investigación.

## Incident

**¿Qué es?**  
Incident es un evento o conjunto de eventos de seguridad que ha sido identificado como una amenaza real o una violación de las políticas de seguridad y requiere respuesta.

**¿Dónde lo encuentro?**  
En SOC, sistemas de gestión de incidentes, SIEM, EDR y procesos formales de Incident Response.

**¿Por qué me afecta?**  
Un incidente puede comprometer la confidencialidad, integridad o disponibilidad de sistemas y datos.

**¿Cómo se soluciona?**  
Aplicando un proceso estructurado de respuesta que incluya análisis, contención, erradicación, recuperación y documentación.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentará ampliar el alcance del incidente antes de ser detectado, comprometiendo más cuentas, sistemas o información.

## Case

**¿Qué es?**  
Case es un registro estructurado utilizado para documentar y gestionar una investigación o incidente de seguridad.

**¿Dónde lo encuentro?**  
En plataformas de gestión de incidentes, SIEM, SOAR, sistemas de ticketing y herramientas utilizadas por equipos SOC.

**¿Por qué me afecta?**  
Permite centralizar evidencia, decisiones, acciones, responsables y resultados relacionados con una investigación.

**¿Cómo se soluciona?**  
Manteniendo el Case actualizado, documentando las acciones realizadas y vinculando las evidencias y alertas relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
No interactúa directamente con el Case, pero puede intentar dificultar la investigación que este documenta eliminando o alterando evidencia en los sistemas afectados.

## Ticket

**¿Qué es?**  
Ticket es un registro utilizado para asignar, rastrear y documentar una tarea, alerta, solicitud o incidente durante su gestión.

**¿Dónde lo encuentro?**  
En sistemas de ticketing, mesas de ayuda, plataformas SOC y herramientas de gestión de incidentes.

**¿Por qué me afecta?**  
Permite controlar responsables, prioridades, tiempos de respuesta y acciones realizadas durante la atención de un evento.

**¿Cómo se soluciona?**  
Asignando correctamente el ticket, documentando las acciones y manteniendo actualizados su estado, prioridad y resolución.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar retrasos, errores de asignación o falta de seguimiento de tickets para prolongar una actividad maliciosa sin ser atendida.

## Escalation

**¿Qué es?**  
Escalation es el proceso de transferir un evento, alerta o incidente a un nivel superior o a un equipo con mayor autoridad, experiencia o capacidad de respuesta.

**¿Dónde lo encuentro?**  
En SOC, Incident Response, sistemas de ticketing y procedimientos de gestión de incidentes.

**¿Por qué me afecta?**  
Una escalación adecuada garantiza que los incidentes de mayor riesgo reciban los recursos y conocimientos necesarios para responder rápidamente.

**¿Cómo se soluciona?**  
Definiendo criterios claros de escalación basados en severidad, impacto, criticidad y alcance del incidente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar mantener sus acciones por debajo de los criterios de escalación para retrasar la intervención de equipos especializados.
