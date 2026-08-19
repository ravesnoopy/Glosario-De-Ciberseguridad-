
## Detection

**¿Qué es?**  
Proceso de identificar actividades, eventos o comportamientos que pueden indicar una amenaza o incidente de seguridad.

**¿Dónde lo encuentro?**  
En SOC, SIEM, EDR, sistemas de monitoreo, registros de eventos, alertas de seguridad y herramientas de análisis.

**¿Por qué me afecta?**  
Una detección tardía puede permitir que un atacante permanezca más tiempo en el entorno y aumente el impacto del incidente.

**¿Cómo se soluciona?**  
Centralizar logs, establecer reglas de detección, monitorear activos críticos y mejorar continuamente las capacidades de análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría ocultar o reducir las señales de su actividad para permanecer en el entorno sin generar alertas.


## Identification

**¿Qué es?**  
Proceso de confirmar que un evento representa un incidente de seguridad y determinar su alcance, causa y recursos afectados.

**¿Dónde lo encuentro?**  
En procesos de respuesta a incidentes, SOC, investigaciones DFIR, análisis de alertas y gestión de incidentes.

**¿Por qué me afecta?**  
Una identificación incorrecta puede provocar que una amenaza real sea ignorada o que los recursos se utilicen sobre una alerta que no representa un incidente.

**¿Cómo se soluciona?**  
Correlacionar evidencias, analizar logs, validar indicadores y determinar qué sistemas, cuentas y datos están involucrados.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría generar actividad que parezca legítima o mezclar sus acciones con tráfico normal para dificultar la identificación del incidente.


## Containment

**¿Qué es?**  
Conjunto de acciones destinadas a limitar la propagación y el impacto de un incidente mientras se investiga y elimina la amenaza.

**¿Dónde lo encuentro?**  
En procesos de respuesta a incidentes, SOC, equipos de seguridad, redes, endpoints y entornos cloud.

**¿Por qué me afecta?**  
Una contención rápida puede evitar que un atacante se mueva lateralmente, acceda a más datos o comprometa otros sistemas.

**¿Cómo se soluciona?**  
Aislar sistemas afectados, bloquear comunicaciones maliciosas, deshabilitar cuentas comprometidas y aplicar otras medidas temporales según el incidente.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría mantener múltiples puntos de acceso o utilizar diferentes identidades para dificultar que la organización pueda contener completamente su presencia.


## Eradication

**¿Qué es?**  
Proceso de eliminar completamente la causa y los componentes maliciosos asociados con un incidente de seguridad.

**¿Dónde lo encuentro?**  
En la fase de respuesta a incidentes, después de contener la amenaza y determinar cómo se produjo el compromiso.

**¿Por qué me afecta?**  
Una erradicación incompleta puede dejar malware, cuentas comprometidas, persistencia o vulnerabilidades que permitan al atacante regresar.

**¿Cómo se soluciona?**  
Eliminar malware y mecanismos de persistencia, corregir vulnerabilidades, revocar credenciales comprometidas y eliminar las causas del incidente.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría mantener mecanismos de persistencia o accesos alternativos para recuperar el control después de que algunas partes de su actividad hayan sido eliminadas.


## Recovery

**¿Qué es?**  
Proceso de restaurar sistemas y operaciones afectadas a un estado seguro y funcional después de controlar y eliminar un incidente.

**¿Dónde lo encuentro?**  
En planes de respuesta y recuperación, continuidad de negocio, recuperación ante desastres y operaciones de TI.

**¿Por qué me afecta?**  
Una recuperación deficiente puede prolongar la interrupción del negocio o reintroducir sistemas comprometidos en producción.

**¿Cómo se soluciona?**  
Restaurar desde fuentes confiables, validar la seguridad de los sistemas, monitorear su comportamiento y recuperar progresivamente las operaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría permanecer oculto durante la recuperación para recuperar acceso cuando los sistemas vuelvan a estar operativos.


## Lessons Learned

**¿Qué es?**  
Proceso posterior a un incidente destinado a analizar qué ocurrió, qué funcionó o falló y qué cambios deben realizarse para evitar incidentes similares.

**¿Dónde lo encuentro?**  
En revisiones posteriores a incidentes, equipos SOC, gestión de riesgos, respuesta a incidentes y programas de mejora continua.

**¿Por qué me afecta?**  
Sin este análisis, una organización puede repetir las mismas deficiencias y mantener vulnerabilidades o procesos que facilitaron el incidente.

**¿Cómo se soluciona?**  
Documentar el incidente, analizar causas y controles, identificar mejoras y convertir los hallazgos en acciones concretas de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Si la organización no aprende de incidentes anteriores, podría reutilizar técnicas o aprovechar las mismas debilidades en futuros ataques.
