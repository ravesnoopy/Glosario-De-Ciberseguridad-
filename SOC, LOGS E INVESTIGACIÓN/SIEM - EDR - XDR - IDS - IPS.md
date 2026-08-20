
## SIEM

**¿Qué es?**  
Security Information and Event Management es una plataforma que centraliza, correlaciona y analiza eventos de seguridad provenientes de múltiples fuentes.

**¿Dónde lo encuentro?**  
En centros de operaciones de seguridad (SOC), conectado a fuentes como firewalls, servidores, endpoints, aplicaciones y servicios cloud.

**¿Por qué me afecta?**  
Proporciona una visión centralizada para detectar amenazas, investigar incidentes y correlacionar actividad entre diferentes sistemas.

**¿Cómo se soluciona?**  
Configurar correctamente las fuentes de logs, reglas de detección, retención, normalización y controles de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría generar actividad que evite las detecciones, mezclarse con tráfico legítimo o aprovechar sistemas que no estén enviando telemetría al SIEM.


## EDR

**¿Qué es?**  
Endpoint Detection and Response es una solución que recopila telemetría de endpoints para detectar, investigar y responder ante comportamientos sospechosos.

**¿Dónde lo encuentro?**  
En estaciones de trabajo, servidores y otros endpoints de una organización.

**¿Por qué me afecta?**  
Permite observar procesos, archivos, conexiones y otras actividades del endpoint que pueden revelar una intrusión.

**¿Cómo se soluciona?**  
Instalar agentes correctamente, mantenerlos actualizados, configurar políticas de detección y asegurar su administración.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría evadir o deshabilitar el agente, utilizar procesos legítimos o ejecutar acciones que se confundan con actividad normal.


## XDR

**¿Qué es?**  
Extended Detection and Response es una estrategia o plataforma que integra y correlaciona señales de diferentes capas, como endpoints, redes, identidades, correo y cloud.

**¿Dónde lo encuentro?**  
En entornos empresariales donde se requiere correlacionar telemetría de múltiples dominios de seguridad.

**¿Por qué me afecta?**  
Permite detectar ataques que atraviesan varios sistemas y proporciona mayor contexto que analizar cada fuente de manera aislada.

**¿Cómo se soluciona?**  
Integrar fuentes relevantes, mantener la telemetría disponible y configurar correctamente las detecciones y respuestas automatizadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría distribuir sus acciones entre diferentes capas para reducir las señales individuales y dificultar su correlación.


## IDS

**¿Qué es?**  
Intrusion Detection System es un sistema que monitorea actividad de red o sistemas para identificar patrones asociados con posibles amenazas y generar alertas.

**¿Dónde lo encuentro?**  
En redes empresariales, segmentos críticos, centros de datos y puntos estratégicos de monitoreo.

**¿Por qué me afecta?**  
Puede detectar escaneos, explotación, tráfico malicioso y otros comportamientos sospechosos antes de que el incidente avance.

**¿Cómo se soluciona?**  
Configurar reglas adecuadas, mantener firmas actualizadas, ajustar falsos positivos y complementar las alertas con otras fuentes.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría modificar su tráfico o comportamiento para evitar las firmas y patrones utilizados por el IDS.


## IPS

**¿Qué es?**  
Intrusion Prevention System es un sistema que detecta actividad potencialmente maliciosa y puede bloquearla o impedir que continúe según las reglas configuradas.

**¿Dónde lo encuentro?**  
En puntos de control de red, firewalls de nueva generación y arquitecturas de seguridad empresariales.

**¿Por qué me afecta?**  
Puede detener determinadas amenazas automáticamente antes de que alcancen los sistemas protegidos.

**¿Cómo se soluciona?**  
Configurar reglas adecuadas, mantener firmas actualizadas, validar bloqueos y controlar los falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría evadir las reglas de inspección mediante cambios en el tráfico, técnicas de ofuscación o utilizando comunicaciones que el IPS no identifique como maliciosas.
