
## Evidence Validation

**¿Qué es?**  
Evidence Validation es el proceso de verificar que una evidencia digital sea auténtica, íntegra, relevante y adecuada para respaldar una conclusión durante una investigación.

**¿Dónde lo encuentro?**  
En investigaciones DFIR, análisis forense, auditorías y procesos de respuesta a incidentes donde las conclusiones deben estar respaldadas por evidencia confiable.

**¿Por qué me afecta?**  
Una evidencia alterada, incompleta o mal interpretada puede conducir a conclusiones incorrectas y afectar la precisión de una investigación.

**¿Cómo se soluciona?**  
Verificando hashes, origen, timestamps, contexto, consistencia y relación con otras fuentes de evidencia antes de utilizarla para respaldar una conclusión.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar modificar, eliminar o falsificar artefactos para generar evidencia engañosa o dificultar la validación de los hechos.

## Chain of Custody

**¿Qué es?**  
Chain of Custody es el registro documentado de la posesión, transferencia, almacenamiento y manipulación de una evidencia desde su recopilación hasta su disposición final.

**¿Dónde lo encuentro?**  
En investigaciones forenses, procesos DFIR y casos donde es necesario demostrar cómo fue manejada una evidencia.

**¿Por qué me afecta?**  
Una cadena de custodia incompleta puede generar dudas sobre la integridad, procedencia o autenticidad de la evidencia.

**¿Cómo se soluciona?**  
Documentando quién recopiló, recibió, almacenó o manipuló la evidencia, junto con fechas, acciones realizadas y mecanismos de integridad cuando correspondan.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar alterar o contaminar evidencia para dificultar posteriormente demostrar su autenticidad o reconstruir los hechos.

## Documentation

**¿Qué es?**  
Documentation es el registro estructurado de actividades, decisiones, evidencias, hallazgos y acciones realizadas durante un proceso de seguridad o investigación.

**¿Dónde lo encuentro?**  
En investigaciones de incidentes, auditorías, procedimientos de seguridad, informes técnicos y sistemas de gestión de incidentes.

**¿Por qué me afecta?**  
Una documentación deficiente dificulta reconstruir lo ocurrido, justificar decisiones y repetir o verificar las acciones realizadas.

**¿Cómo se soluciona?**  
Registrando de forma clara las acciones, fechas, responsables, evidencias, decisiones y resultados relevantes durante todo el proceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar la falta de documentación para dificultar la investigación, ocultar cambios realizados o explotar procedimientos que no estén claramente definidos.

## Executive Summary

**¿Qué es?**  
Executive Summary es una sección breve de un informe que presenta los principales hallazgos, impacto, riesgos y recomendaciones de manera comprensible para responsables de toma de decisiones.

**¿Dónde lo encuentro?**  
En informes de incidentes, auditorías de seguridad, evaluaciones de riesgo y reportes dirigidos a equipos directivos.

**¿Por qué me afecta?**  
Permite que quienes toman decisiones comprendan rápidamente la situación y asignen recursos para atender los riesgos más importantes.

**¿Cómo se soluciona?**  
Presentando el impacto, nivel de riesgo, causas principales y acciones recomendadas de forma clara, concisa y orientada al negocio.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar que los responsables no comprendan la gravedad de un incidente si la información crítica se comunica de forma incompleta o poco clara.

## Technical Finding

**¿Qué es?**  
Technical Finding es un hallazgo técnico identificado durante una evaluación, auditoría o investigación que demuestra una condición relevante de seguridad.

**¿Dónde lo encuentro?**  
En informes de vulnerabilidades, auditorías, pruebas de seguridad, investigaciones de incidentes y evaluaciones de infraestructura.

**¿Por qué me afecta?**  
Un hallazgo técnico puede revelar una vulnerabilidad, configuración insegura, exposición o comportamiento que represente un riesgo para la organización.

**¿Cómo se soluciona?**  
Documentando claramente la evidencia, causa, impacto y contexto del hallazgo para facilitar la selección de una medida correctiva adecuada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede identificar la misma debilidad mediante reconocimiento o explotación y utilizarla como parte de una cadena de ataque.

## Recommendation

**¿Qué es?**  
Recommendation es una acción propuesta para reducir un riesgo, corregir un hallazgo o mejorar una condición de seguridad identificada.

**¿Dónde lo encuentro?**  
En informes de auditoría, evaluaciones de seguridad, investigaciones de incidentes y planes de mejora.

**¿Por qué me afecta?**  
Una recomendación clara permite convertir un hallazgo en una acción concreta para reducir la exposición al riesgo.

**¿Cómo se soluciona?**  
Definiendo acciones específicas, responsables, prioridades y criterios que permitan verificar su implementación y efectividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede beneficiarse de recomendaciones que no sean implementadas o de controles que permanezcan débiles después de haber sido identificados.

## Remediation

**¿Qué es?**  
Remediation es el proceso de corregir una vulnerabilidad, debilidad o condición de seguridad para reducir o eliminar el riesgo asociado.

**¿Dónde lo encuentro?**  
En gestión de vulnerabilidades, respuesta a incidentes, auditorías, hardening y procesos de mejora de seguridad.

**¿Por qué me afecta?**  
Identificar un problema sin corregirlo deja abierta la posibilidad de que un atacante continúe explotándolo.

**¿Cómo se soluciona?**  
Aplicando la corrección correspondiente, verificando que haya eliminado o reducido el riesgo y realizando una nueva evaluación cuando sea necesario.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar una vulnerabilidad conocida que permanece sin corregir para obtener acceso, escalar privilegios o mantener presencia.

## Lessons Learned

**¿Qué es?**  
Lessons Learned es el proceso de identificar conocimientos y mejoras obtenidos después de un incidente, investigación, ejercicio o proyecto de seguridad.

**¿Dónde lo encuentro?**  
En revisiones posteriores a incidentes, informes DFIR, ejercicios de respuesta y procesos de mejora continua.

**¿Por qué me afecta?**  
Permite evitar que los mismos errores vuelvan a ocurrir y mejorar controles, procedimientos y capacidades de respuesta.

**¿Cómo se soluciona?**  
Documentando qué funcionó, qué falló y qué debe cambiar, y convirtiendo esas conclusiones en acciones concretas de mejora.

**¿Cómo lo usaría un atacante en mi contra?**  
Si una organización no aprende de incidentes anteriores, puede repetir las mismas debilidades y ofrecer al atacante una ruta conocida para comprometerla nuevamente.
