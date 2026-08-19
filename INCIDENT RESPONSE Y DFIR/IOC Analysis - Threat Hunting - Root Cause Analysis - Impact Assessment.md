
## IOC Analysis

**¿Qué es?**  
Proceso de analizar Indicadores de Compromiso (IOC) como hashes, direcciones IP, dominios, URLs o nombres de archivos para identificar posibles actividades maliciosas.

**¿Dónde lo encuentro?**  
En investigaciones de incidentes, alertas del SOC, logs, EDR, SIEM, inteligencia de amenazas y evidencias forenses.

**¿Por qué me afecta?**  
Permite determinar si otros sistemas presentan evidencias relacionadas con una amenaza y ayuda a ampliar el alcance de una investigación.

**¿Cómo se soluciona?**  
Correlacionar los IOC con múltiples fuentes, validar su contexto y actualizar las detecciones cuando se confirme actividad maliciosa.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría cambiar o reutilizar infraestructura, archivos o indicadores para dificultar que sus actividades sean identificadas mediante IOC conocidos.


## Threat Hunting

**¿Qué es?**  
Proceso proactivo de buscar amenazas o comportamientos sospechosos dentro de un entorno aunque no exista una alerta específica que indique un compromiso.

**¿Dónde lo encuentro?**  
En SOC, equipos de threat intelligence, EDR, SIEM, análisis de logs y operaciones de detección y respuesta.

**¿Por qué me afecta?**  
Permite encontrar actividad maliciosa que los controles automáticos no detectaron y descubrir compromisos que podrían permanecer ocultos.

**¿Cómo se soluciona?**  
Definir hipótesis de búsqueda, analizar telemetría relevante, correlacionar comportamientos y convertir los hallazgos en nuevas detecciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría mantener un comportamiento similar al de usuarios o sistemas legítimos para evitar generar patrones suficientemente anómalos durante las búsquedas.


## Root Cause Analysis

**¿Qué es?**  
Proceso de determinar la causa fundamental que permitió que ocurriera un incidente o problema de seguridad, más allá de identificar únicamente sus consecuencias.

**¿Dónde lo encuentro?**  
En investigaciones de incidentes, análisis posteriores, gestión de vulnerabilidades, auditorías y procesos de mejora continua.

**¿Por qué me afecta?**  
Si solo se corrige el síntoma y no la causa raíz, la misma vulnerabilidad, configuración o deficiencia puede permitir otro incidente.

**¿Cómo se soluciona?**  
Analizar la secuencia de eventos, identificar las condiciones que hicieron posible el incidente y corregir las causas técnicas o procedimentales.

**¿Cómo lo usaría un atacante en mi contra?**  
Si una causa raíz permanece sin corregir, podría reutilizar la misma debilidad para obtener acceso nuevamente o comprometer otros sistemas.


## Impact Assessment

**¿Qué es?**  
Proceso de determinar las consecuencias de un incidente sobre sistemas, datos, operaciones, usuarios y objetivos del negocio.

**¿Dónde lo encuentro?**  
En respuesta a incidentes, gestión de riesgos, continuidad de negocio, análisis forense y procesos de recuperación.

**¿Por qué me afecta?**  
Permite establecer la gravedad del incidente, priorizar acciones de respuesta y determinar qué recursos necesitan recuperación inmediata.

**¿Cómo se soluciona?**  
Identificar activos afectados, evaluar el alcance y las consecuencias y priorizar la recuperación según la criticidad de los recursos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometer activos de alto impacto o información crítica para maximizar las consecuencias operativas, financieras o reputacionales.
