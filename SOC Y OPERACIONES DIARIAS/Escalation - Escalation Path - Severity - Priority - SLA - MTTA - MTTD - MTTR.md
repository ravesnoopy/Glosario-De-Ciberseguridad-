
## Escalation

**¿Qué es?**  
Proceso mediante el cual una alerta, incidente o caso se eleva a un nivel superior de atención debido a su gravedad, complejidad o impacto.

**¿Dónde lo encuentro?**  
En SOC, equipos de respuesta a incidentes, ITSM y procesos de gestión de incidentes.

**¿Por qué me afecta?**  
Una escalación tardía puede retrasar la contención y aumentar el impacto de un incidente.

**¿Cómo se soluciona?**  
Definir criterios claros de escalación basados en severidad, impacto, alcance y nivel de acceso involucrado.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría mantener una actividad por debajo de los criterios de escalación para retrasar la intervención de analistas con mayores privilegios.


## Escalation Path

**¿Qué es?**  
Ruta definida que establece a qué persona, equipo o nivel de especialización debe escalarse un caso según determinadas condiciones.

**¿Dónde lo encuentro?**  
En procedimientos de SOC, playbooks, sistemas de tickets y procesos de respuesta a incidentes.

**¿Por qué me afecta?**  
Una ruta incorrecta puede provocar que un incidente llegue tarde al equipo capaz de contenerlo.

**¿Cómo se soluciona?**  
Definir responsables, criterios de escalación, canales de comunicación y niveles de atención claramente.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar retrasos o confusión sobre quién debe recibir un caso para prolongar su actividad.


## Severity

**¿Qué es?**  
Medida que representa la gravedad técnica o potencial impacto de una alerta, vulnerabilidad o incidente.

**¿Dónde lo encuentro?**  
En SIEM, EDR, sistemas de tickets, gestión de vulnerabilidades y procesos de respuesta a incidentes.

**¿Por qué me afecta?**  
Ayuda a determinar qué incidentes requieren atención inmediata y cuáles pueden ser tratados posteriormente.

**¿Cómo se soluciona?**  
Establecer criterios consistentes considerando factores como impacto, alcance, criticidad del activo y naturaleza de la amenaza.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar ocultar actividad maliciosa dentro de eventos de baja severidad para evitar una respuesta rápida.


## Priority

**¿Qué es?**  
Nivel de urgencia asignado a una tarea, alerta o incidente para determinar el orden en que debe ser atendido.

**¿Dónde lo encuentro?**  
En sistemas de tickets, SOC, ITSM y plataformas de gestión de incidentes.

**¿Por qué me afecta?**  
Una prioridad incorrecta puede hacer que un incidente crítico sea atendido después de casos menos importantes.

**¿Cómo se soluciona?**  
Establecer criterios objetivos basados en impacto, urgencia, criticidad del activo y riesgo.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría generar ruido o actividad aparentemente prioritaria para desviar la atención de acciones más relevantes.


## SLA

**¿Qué es?**  
Service Level Agreement es un acuerdo que establece niveles de servicio, tiempos de respuesta y compromisos entre las partes involucradas.

**¿Dónde lo encuentro?**  
En servicios gestionados, SOC, proveedores de seguridad, ITSM y contratos de servicios tecnológicos.

**¿Por qué me afecta?**  
Define expectativas sobre cuánto tiempo puede transcurrir antes de responder o resolver determinados eventos.

**¿Cómo se soluciona?**  
Establecer objetivos medibles, monitorear su cumplimiento y definir escalaciones ante incumplimientos.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar retrasos operativos o tiempos de respuesta elevados para mantener actividad maliciosa durante más tiempo.


## MTTA

**¿Qué es?**  
Mean Time to Acknowledge es el tiempo promedio que transcurre desde que se genera una alerta o incidente hasta que un analista confirma que ha sido recibido y atendido.

**¿Dónde lo encuentro?**  
En métricas de SOC, SIEM, plataformas de tickets y sistemas de gestión de incidentes.

**¿Por qué me afecta?**  
Un MTTA elevado indica que las alertas pueden permanecer sin atención durante demasiado tiempo.

**¿Cómo se soluciona?**  
Mejorar el monitoreo, priorización, asignación automática y procesos de escalación de alertas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría aprovechar periodos prolongados sin atención para ejecutar acciones antes de que un analista intervenga.


## MTTD

**¿Qué es?**  
Mean Time to Detect es el tiempo promedio que transcurre desde que comienza una actividad o incidente hasta que es detectado por la organización.

**¿Dónde lo encuentro?**  
En métricas de SOC, respuesta a incidentes, SIEM, EDR y programas de detección.

**¿Por qué me afecta?**  
Un MTTD elevado significa que un atacante puede permanecer activo durante más tiempo antes de ser identificado.

**¿Cómo se soluciona?**  
Mejorar la telemetría, detecciones, correlación de eventos, Threat Hunting y monitoreo continuo.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría permanecer dentro del entorno durante periodos prolongados evitando comportamientos que generen detecciones.


## MTTR

**¿Qué es?**  
Mean Time to Respond o Mean Time to Recover, según el contexto, representa el tiempo promedio necesario para responder a un incidente o recuperar el servicio afectado.

**¿Dónde lo encuentro?**  
En métricas de SOC, respuesta a incidentes, operaciones de TI y gestión de disponibilidad.

**¿Por qué me afecta?**  
Un MTTR elevado puede aumentar el tiempo durante el cual un atacante mantiene impacto o acceso al entorno.

**¿Cómo se soluciona?**  
Mejorar playbooks, automatización, escalación, coordinación entre equipos y procedimientos de recuperación.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar una respuesta o recuperación lenta para prolongar el impacto del incidente y ampliar sus oportunidades dentro del entorno.
