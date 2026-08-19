
## False Positive

**¿Qué es?**  
False Positive es una alerta que indica una posible actividad maliciosa cuando, después de analizarla, se determina que la actividad era legítima.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, antivirus y otras herramientas que generan alertas de seguridad.

**¿Por qué me afecta?**  
Un volumen elevado de falsos positivos puede generar Alert Fatigue y hacer que los analistas pasen por alto amenazas reales.

**¿Cómo se soluciona?**  
Ajustando las reglas de detección, agregando contexto y excepciones apropiadas y revisando periódicamente los patrones de actividad legítima.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede generar actividad que produzca numerosos falsos positivos para crear ruido y dificultar la identificación de sus acciones maliciosas.

## True Positive

**¿Qué es?**  
True Positive es una alerta que identifica correctamente una actividad que realmente corresponde a un comportamiento malicioso o una condición de seguridad que requiere atención.

**¿Dónde lo encuentro?**  
En SIEM, EDR, IDS, antivirus y procesos de monitoreo y respuesta de seguridad.

**¿Por qué me afecta?**  
Representa una señal válida que puede indicar un ataque, compromiso o actividad que requiere investigación y respuesta.

**¿Cómo se soluciona?**  
Validando la alerta, determinando su alcance e impacto y aplicando las acciones de respuesta y remediación correspondientes.

**¿Cómo lo usaría un atacante en mi contra?**  
Un atacante intentará evitar generar señales que coincidan con las condiciones de detección y utilizará técnicas que reduzcan la probabilidad de producir un True Positive.
