
## Threat Feed

**¿Qué es?**  
Threat Feed es una fuente que proporciona información actualizada sobre amenazas, como IOCs, dominios, direcciones IP, hashes o actividad de actores maliciosos.

**¿Dónde lo encuentro?**  
En plataformas de threat intelligence, SIEM, EDR y servicios que distribuyen información de amenazas para integrarla en controles de seguridad.

**¿Por qué me afecta?**  
Permite incorporar información externa sobre amenazas y mejorar la capacidad de identificar actividad potencialmente maliciosa.

**¿Cómo se soluciona?**  
Utilizando fuentes confiables, evaluando la calidad de la información y automatizando su integración cuando sea apropiado.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cambiar sus indicadores o infraestructura para evitar aparecer en feeds de amenazas conocidos.

## Indicator

**¿Qué es?**  
Un Indicator es un dato observable que puede proporcionar información sobre una amenaza o actividad relacionada con ella, como una dirección IP, dominio, hash o URL.

**¿Dónde lo encuentro?**  
En logs, EDR, SIEM, tráfico de red, análisis forense y fuentes de threat intelligence.

**¿Por qué me afecta?**  
Permite relacionar actividad observada con posibles amenazas y apoyar procesos de detección e investigación.

**¿Cómo se soluciona?**  
Recopilando indicadores relevantes, validándolos y utilizándolos junto con contexto y análisis de comportamiento.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar o reemplazar sus indicadores para evitar detecciones basadas en valores conocidos.

## Reputation

**¿Qué es?**  
Reputation es la evaluación del nivel de confianza o riesgo asociado a un indicador, dominio, dirección IP, archivo u otra entidad según información disponible.

**¿Dónde lo encuentro?**  
En servicios de threat intelligence, filtros de correo, sistemas de seguridad, navegadores y herramientas de análisis de amenazas.

**¿Por qué me afecta?**  
Puede ayudar a identificar rápidamente recursos potencialmente maliciosos y priorizar investigaciones o bloqueos.

**¿Cómo se soluciona?**  
Utilizando fuentes de reputación confiables y combinando la reputación con contexto y otras evidencias antes de tomar decisiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar infraestructura nueva, comprometida o con buena reputación para reducir la probabilidad de ser detectado.

## Attribution

**¿Qué es?**  
Attribution es el proceso de evaluar y relacionar una actividad maliciosa con un posible actor, grupo, organización o infraestructura.

**¿Dónde lo encuentro?**  
En threat intelligence, investigaciones de incidentes y análisis de campañas y grupos adversarios.

**¿Por qué me afecta?**  
Puede ayudar a comprender motivaciones, capacidades y patrones de un adversario, aunque la atribución suele tener distintos niveles de confianza.

**¿Cómo se soluciona?**  
Correlacionando múltiples evidencias como TTP, infraestructura, malware, objetivos y patrones de actividad, evitando basarse en un único indicador.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar infraestructura compartida, técnicas comunes o información engañosa para dificultar o confundir la atribución de sus actividades.

## Infrastructure

**¿Qué es?**  
Infrastructure es el conjunto de recursos técnicos utilizados para operar, controlar, distribuir o apoyar una actividad, incluyendo dominios, direcciones IP, servidores y otros servicios.

**¿Dónde lo encuentro?**  
En análisis de amenazas, investigaciones de incidentes, DNS, registros de red, threat intelligence y análisis de infraestructura adversaria.

**¿Por qué me afecta?**  
La infraestructura puede revelar conexiones entre diferentes actividades y proporcionar oportunidades para detectar o bloquear operaciones maliciosas.

**¿Cómo se soluciona?**  
Monitoreando dominios, IPs, DNS, certificados y otros recursos relevantes, y correlacionándolos con inteligencia y actividad observada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar infraestructura desechable, comprometida o distribuida para alojar malware, establecer C2 y dificultar su identificación.
