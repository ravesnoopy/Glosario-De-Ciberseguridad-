
## Incident Classification

**¿Qué es?**  
Incident Classification es el proceso de determinar qué tipo de incidente de seguridad ocurrió según la evidencia disponible y su naturaleza.

**¿Dónde lo encuentro?**  
En procedimientos de Incident Response, SOC, sistemas de ticketing, SIEM y documentación de incidentes.

**¿Por qué me afecta?**  
Una clasificación incorrecta puede provocar que un incidente reciba una respuesta inadecuada o que no se involucren los equipos necesarios.

**¿Cómo se soluciona?**  
Definiendo categorías claras, criterios consistentes y procedimientos para clasificar los incidentes según la evidencia disponible.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar ocultar sus actividades entre eventos aparentemente legítimos para dificultar su correcta clasificación.

## Incident Categorization

**¿Qué es?**  
Incident Categorization es la asignación de un incidente a una categoría específica, como malware, phishing, acceso no autorizado o compromiso de credenciales.

**¿Dónde lo encuentro?**  
En sistemas de gestión de incidentes, SOC, plataformas de ticketing y procedimientos de respuesta.

**¿Por qué me afecta?**  
Ayuda a determinar qué procedimientos, herramientas y especialistas deben participar en la respuesta.

**¿Cómo se soluciona?**  
Estableciendo categorías bien definidas y utilizando evidencia técnica para asignar cada incidente a la categoría correspondiente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar técnicas que mezclen diferentes tipos de actividad para dificultar la identificación de la categoría real del incidente.

## Incident Severity

**¿Qué es?**  
Incident Severity es el nivel de gravedad asignado a un incidente según factores como impacto, alcance, criticidad de los activos y riesgo para la organización.

**¿Dónde lo encuentro?**  
En SOC, sistemas de gestión de incidentes, procedimientos de Incident Response y plataformas de ticketing.

**¿Por qué me afecta?**  
Determina la prioridad de respuesta y los recursos que deben asignarse para contener y resolver el incidente.

**¿Cómo se soluciona?**  
Definiendo criterios objetivos de severidad y reevaluándolos conforme aparece nueva evidencia durante la investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede mantener inicialmente sus acciones en un nivel de bajo impacto para retrasar la escalada del incidente y posteriormente aumentar su alcance.

## Incident Ownership

**¿Qué es?**  
Incident Ownership es la asignación de responsabilidad sobre la coordinación y gestión de un incidente durante su investigación y respuesta.

**¿Dónde lo encuentro?**  
En SOC, equipos de Incident Response, sistemas de ticketing y procedimientos internos de gestión de incidentes.

**¿Por qué me afecta?**  
Un incidente sin un responsable claro puede generar retrasos, duplicación de esfuerzos o falta de coordinación durante la respuesta.

**¿Cómo se soluciona?**  
Asignando un responsable definido, estableciendo roles y documentando las acciones y decisiones tomadas durante el incidente.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar confusión entre equipos o falta de responsabilidad clara para retrasar la respuesta y mantener su acceso.

## Detection

**¿Qué es?**  
Detection es la capacidad de identificar una actividad, evento o comportamiento que puede indicar una amenaza o condición de seguridad relevante.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, NDR, sistemas de monitoreo y procesos de Threat Hunting.

**¿Por qué me afecta?**  
Una detección efectiva permite identificar actividad maliciosa antes de que produzca un impacto mayor.

**¿Cómo se soluciona?**  
Mejorando la telemetría, desarrollando reglas adecuadas, validando las detecciones y revisando continuamente su cobertura.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentará modificar o esconder su comportamiento para evitar las condiciones que activan las detecciones disponibles.

## Detection Rule

**¿Qué es?**  
Detection Rule es una regla que define condiciones específicas que, cuando se cumplen, indican una actividad potencialmente sospechosa y pueden generar una alerta.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, NDR y otras plataformas de seguridad.

**¿Por qué me afecta?**  
Las reglas de detección convierten los datos de seguridad en señales que los analistas pueden investigar.

**¿Cómo se soluciona?**  
Diseñando reglas basadas en comportamientos relevantes, probándolas con datos reales y ajustándolas para mantener una cobertura adecuada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cambiar sus técnicas, parámetros o patrones de actividad para evitar coincidir con las condiciones definidas en una regla.

## Detection Logic

**¿Qué es?**  
Detection Logic es el conjunto de condiciones y relaciones utilizadas para determinar cuándo una actividad debe considerarse sospechosa y generar una detección.

**¿Dónde lo encuentro?**  
En reglas SIEM, consultas de detección, EDR, sistemas de monitoreo y herramientas de Threat Hunting.

**¿Por qué me afecta?**  
Una lógica deficiente puede producir falsos positivos o dejar actividades maliciosas fuera de la cobertura de detección.

**¿Cómo se soluciona?**  
Validando las condiciones con datos reales, incorporando contexto relevante y ajustando la lógica según los resultados de las investigaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede adaptar su comportamiento para evitar las condiciones específicas que forman parte de la lógica de detección.
