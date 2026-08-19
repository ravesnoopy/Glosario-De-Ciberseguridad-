
## Attack Chain

**¿Qué es?**  
Attack Chain es la representación de las diferentes etapas y acciones que un atacante puede seguir desde el acceso inicial hasta alcanzar sus objetivos.

**¿Dónde lo encuentro?**  
En análisis de incidentes, threat intelligence, ejercicios de seguridad y documentación utilizada para reconstruir ataques.

**¿Por qué me afecta?**  
Permite entender cómo progresa un ataque y dónde existen oportunidades para prevenirlo, detectarlo o detenerlo.

**¿Cómo se soluciona?**  
Mapeando las acciones observadas, identificando controles y detecciones para cada etapa y corrigiendo las debilidades que permiten avanzar al atacante.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede encadenar diferentes técnicas para avanzar desde el acceso inicial hasta objetivos como robo de información, persistencia o interrupción de servicios.

## Kill Chain

**¿Qué es?**  
Kill Chain es un modelo que divide un ataque en etapas para analizar cómo se desarrolla y determinar puntos donde puede ser interrumpido.

**¿Dónde lo encuentro?**  
En análisis de amenazas, threat intelligence, operaciones de seguridad y metodologías utilizadas para estudiar campañas de ataque.

**¿Por qué me afecta?**  
Ayuda a identificar oportunidades de detección y prevención antes de que un atacante alcance su objetivo final.

**¿Cómo se soluciona?**  
Implementando controles de seguridad y detecciones en diferentes etapas del ataque, evitando depender de una única capa defensiva.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar completar cada etapa sin ser detectado, adaptando sus técnicas cuando encuentra controles defensivos.

## MITRE ATT&CK

**¿Qué es?**  
MITRE ATT&CK es una base de conocimiento que documenta tácticas y técnicas utilizadas por adversarios reales para describir y analizar comportamientos de ataque.

**¿Dónde lo encuentro?**  
En análisis de amenazas, detección, threat hunting, evaluación de controles, respuesta a incidentes y documentación de seguridad.

**¿Por qué me afecta?**  
Permite utilizar una terminología común para identificar comportamientos de atacantes y relacionarlos con detecciones y controles defensivos.

**¿Cómo se soluciona?**  
Mapeando comportamientos observados a técnicas y tácticas relevantes y utilizando esa información para desarrollar y evaluar detecciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar cualquiera de las técnicas documentadas en ATT&CK para alcanzar sus objetivos, dependiendo de las características y defensas del entorno.

## Technique

**¿Qué es?**  
Una Technique en MITRE ATT&CK describe un método específico que un adversario puede utilizar para alcanzar un objetivo dentro de una táctica determinada.

**¿Dónde lo encuentro?**  
En MITRE ATT&CK y en análisis de amenazas donde se clasifican comportamientos observados durante ataques.

**¿Por qué me afecta?**  
Identificar técnicas permite comprender qué comportamiento realizó un atacante y desarrollar controles o detecciones específicos.

**¿Cómo se soluciona?**  
Analizando las técnicas relevantes para el entorno y creando controles y detecciones capaces de identificar su ejecución.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede seleccionar una técnica que sea compatible con sus permisos, acceso disponible y características del sistema objetivo.

## Sub-Technique

**¿Qué es?**  
Una Sub-Technique es una categoría más específica dentro de una Technique de MITRE ATT&CK que describe una variante concreta de un comportamiento de ataque.

**¿Dónde lo encuentro?**  
En MITRE ATT&CK, donde determinadas técnicas están divididas en sub-técnicas para proporcionar mayor nivel de detalle.

**¿Por qué me afecta?**  
Permite distinguir diferentes formas de realizar una misma técnica y mejorar la precisión del análisis y las detecciones.

**¿Cómo se soluciona?**  
Identificando correctamente la sub-técnica utilizada y desarrollando detecciones y controles adecuados al comportamiento específico.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede elegir una sub-técnica que aproveche una característica concreta del sistema o que tenga menor probabilidad de ser detectada.

## Tactic

**¿Qué es?**  
Una Tactic en MITRE ATT&CK representa el objetivo que un adversario intenta alcanzar durante una etapa de una operación.

**¿Dónde lo encuentro?**  
En MITRE ATT&CK y en análisis de ataques donde las actividades del adversario se agrupan según sus objetivos.

**¿Por qué me afecta?**  
Permite comprender la intención detrás de una actividad y relacionarla con otras acciones realizadas durante el ataque.

**¿Cómo se soluciona?**  
Analizando las tácticas presentes en el entorno y asegurando que existan controles y detecciones para las diferentes etapas de un ataque.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar diferentes técnicas dentro de una misma táctica para alcanzar un objetivo, adaptándose a las defensas encontradas.

## Procedure

**¿Qué es?**  
Una Procedure en MITRE ATT&CK describe cómo un grupo o software específico ha utilizado una técnica o sub-técnica en operaciones conocidas.

**¿Dónde lo encuentro?**  
En las páginas de técnicas, sub-técnicas, grupos y software de MITRE ATT&CK.

**¿Por qué me afecta?**  
Ayuda a relacionar una técnica abstracta con comportamientos observados en ataques reales, facilitando el análisis y la detección.

**¿Cómo se soluciona?**  
Utilizando procedimientos documentados como referencia para crear hipótesis de threat hunting y detecciones basadas en comportamientos conocidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar procedimientos similares a los documentados por grupos o herramientas conocidas para ejecutar técnicas contra un entorno objetivo.
