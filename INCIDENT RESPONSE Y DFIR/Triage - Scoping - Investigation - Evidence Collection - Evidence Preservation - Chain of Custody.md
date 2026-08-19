
## Triage

**¿Qué es?**  
Triage es el proceso inicial de evaluar una alerta o incidente para determinar su gravedad, prioridad y necesidad de respuesta.

**¿Dónde lo encuentro?**  
En SOC, equipos de respuesta a incidentes y procesos DFIR donde se reciben alertas provenientes de SIEM, EDR, firewalls u otras fuentes.

**¿Por qué me afecta?**  
Un triage incorrecto puede hacer que un incidente crítico sea ignorado o que los recursos se concentren en eventos de menor importancia.

**¿Cómo se soluciona?**  
Estableciendo criterios de severidad, priorizando según impacto y contexto, y recopilando rápidamente la información necesaria para tomar una decisión.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar actividad que parezca legítima o producir múltiples eventos para dificultar la priorización y desviar la atención de sus acciones principales.

## Scoping

**¿Qué es?**  
Scoping es el proceso de determinar el alcance de un incidente, identificando los sistemas, cuentas, datos y recursos potencialmente afectados.

**¿Dónde lo encuentro?**  
En investigaciones de incidentes, procesos DFIR y actividades de respuesta realizadas después de confirmar una amenaza.

**¿Por qué me afecta?**  
Determinar correctamente el alcance evita dejar sistemas comprometidos fuera de la respuesta y permite dimensionar adecuadamente el impacto.

**¿Cómo se soluciona?**  
Correlacionando registros, indicadores de compromiso, actividad de cuentas, endpoints, tráfico de red y otros datos relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer varios sistemas o utilizar diferentes técnicas para dificultar la identificación completa de su presencia dentro del entorno.

## Investigation

**¿Qué es?**  
Investigation es el proceso de analizar información y evidencia para determinar qué ocurrió, cómo ocurrió, qué sistemas fueron afectados y qué acciones realizó un atacante.

**¿Dónde lo encuentro?**  
En SOC, DFIR, análisis forense digital y respuesta a incidentes.

**¿Por qué me afecta?**  
Una investigación adecuada permite comprender la causa y el impacto del incidente, además de identificar mecanismos de compromiso y persistencia.

**¿Cómo se soluciona?**  
Analizando evidencia de múltiples fuentes, construyendo una línea temporal y correlacionando eventos para reconstruir las acciones relevantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar técnicas de evasión, borrar evidencia o mezclarse con actividad legítima para dificultar la reconstrucción de sus acciones.

## Evidence Collection

**¿Qué es?**  
Evidence Collection es el proceso de recopilar datos relevantes para una investigación de seguridad de manera controlada y documentada.

**¿Dónde lo encuentro?**  
En investigaciones DFIR, análisis forense de endpoints, servidores, redes, cuentas y otros sistemas afectados.

**¿Por qué me afecta?**  
Una recopilación incompleta puede provocar que se pierdan datos necesarios para determinar el origen, alcance y evolución de un incidente.

**¿Cómo se soluciona?**  
Identificando las fuentes relevantes, utilizando herramientas apropiadas, documentando las acciones realizadas y preservando la integridad de los datos recopilados.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede eliminar, modificar o sobrescribir información antes de que sea recopilada para dificultar la investigación.

## Evidence Preservation

**¿Qué es?**  
Evidence Preservation es el proceso de proteger la evidencia digital contra modificaciones, pérdida o contaminación durante una investigación.

**¿Dónde lo encuentro?**  
En investigaciones forenses, respuesta a incidentes y procedimientos donde la integridad de la evidencia es importante.

**¿Por qué me afecta?**  
Una evidencia alterada o contaminada puede perder valor para determinar qué ocurrió y cuándo ocurrió.

**¿Cómo se soluciona?**  
Utilizando procedimientos forenses, controles de acceso, hashes, copias verificadas y documentación de las acciones realizadas sobre la evidencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar modificar timestamps, eliminar archivos, borrar registros o alterar otros artefactos para dificultar la preservación y análisis de evidencia.

## Chain of Custody

**¿Qué es?**  
Chain of Custody es el registro documentado de la posesión, transferencia, almacenamiento y manipulación de una evidencia desde su recopilación hasta su disposición final.

**¿Dónde lo encuentro?**  
En investigaciones forenses, procesos DFIR y casos donde es necesario demostrar que la evidencia se mantuvo bajo control adecuado.

**¿Por qué me afecta?**  
Una cadena de custodia deficiente puede generar dudas sobre la integridad y procedencia de la evidencia utilizada durante una investigación.

**¿Cómo se soluciona?**  
Documentando quién recopiló, recibió, almacenó o manipuló la evidencia, junto con fechas, acciones realizadas y mecanismos de integridad cuando correspondan.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar alterar o contaminar evidencia durante el incidente para dificultar posteriormente demostrar su autenticidad o reconstruir los hechos.
