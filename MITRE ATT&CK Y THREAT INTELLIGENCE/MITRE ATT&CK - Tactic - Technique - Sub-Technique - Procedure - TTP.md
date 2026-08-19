
## MITRE ATT&CK

**¿Qué es?**  
MITRE ATT&CK es una base de conocimiento de tácticas y técnicas utilizadas por adversarios durante operaciones de ataque, basada en observaciones del mundo real.

**¿Dónde lo encuentro?**  
En threat intelligence, threat hunting, detección de amenazas, análisis de incidentes y evaluación de controles de seguridad.

**¿Por qué me afecta?**  
Permite describir el comportamiento de los atacantes con una terminología común y relacionarlo con posibles detecciones y controles defensivos.

**¿Cómo se soluciona?**  
Mapeando las actividades observadas a tácticas, técnicas y sub-técnicas relevantes para mejorar la detección y el análisis.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar cualquiera de los comportamientos documentados en ATT&CK para alcanzar sus objetivos, dependiendo del acceso y las características del entorno.

## Tactic

**¿Qué es?**  
Una Tactic en MITRE ATT&CK representa el objetivo que un adversario intenta alcanzar durante una etapa de una operación.

**¿Dónde lo encuentro?**  
En MITRE ATT&CK y en análisis de ataques donde las actividades del adversario se agrupan según sus objetivos.

**¿Por qué me afecta?**  
Permite comprender la intención detrás de una actividad y relacionarla con otras acciones realizadas durante un ataque.

**¿Cómo se soluciona?**  
Analizando las tácticas relevantes para el entorno y asegurando que existan controles y detecciones para las diferentes etapas de un ataque.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar diferentes técnicas dentro de una misma táctica para alcanzar un objetivo y adaptarse a las defensas encontradas.

## Technique

**¿Qué es?**  
Una Technique en MITRE ATT&CK describe un método específico que un adversario puede utilizar para alcanzar un objetivo dentro de una táctica determinada.

**¿Dónde lo encuentro?**  
En MITRE ATT&CK y en análisis de amenazas donde se clasifican comportamientos observados durante ataques.

**¿Por qué me afecta?**  
Identificar técnicas permite comprender qué comportamiento realizó un atacante y desarrollar controles o detecciones específicos.

**¿Cómo se soluciona?**  
Identificando las técnicas relevantes para el entorno y desarrollando controles y detecciones capaces de detectar esos comportamientos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede seleccionar una técnica compatible con sus permisos, acceso disponible y características del sistema objetivo.

## Sub-Technique

**¿Qué es?**  
Una Sub-Technique es una categoría más específica dentro de una Technique de MITRE ATT&CK que describe una variante concreta de un comportamiento de ataque.

**¿Dónde lo encuentro?**  
En MITRE ATT&CK, donde determinadas técnicas se dividen en sub-técnicas para proporcionar mayor precisión.

**¿Por qué me afecta?**  
Permite distinguir diferentes formas de realizar una misma técnica y mejorar la precisión del análisis y las detecciones.

**¿Cómo se soluciona?**  
Identificando correctamente la sub-técnica utilizada y desarrollando detecciones y controles adecuados al comportamiento específico.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede elegir una sub-técnica que aproveche una característica concreta del sistema o tenga menor probabilidad de ser detectada.

## Procedure

**¿Qué es?**  
Una Procedure en MITRE ATT&CK describe cómo un grupo, software u otro componente relacionado con un adversario ha utilizado una técnica o sub-técnica en una operación conocida.

**¿Dónde lo encuentro?**  
En las páginas de técnicas, sub-técnicas, grupos y software de MITRE ATT&CK.

**¿Por qué me afecta?**  
Ayuda a relacionar una técnica abstracta con comportamientos observados en ataques reales, facilitando el análisis y la creación de detecciones.

**¿Cómo se soluciona?**  
Utilizando procedimientos documentados como referencia para crear hipótesis de threat hunting y detecciones basadas en comportamientos conocidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede emplear procedimientos similares a los documentados para ejecutar técnicas contra un entorno objetivo.

## TTP

**¿Qué es?**  
TTP (Tactics, Techniques and Procedures) describe las tácticas, técnicas y procedimientos que utiliza un adversario para realizar sus operaciones.

**¿Dónde lo encuentro?**  
En threat intelligence, MITRE ATT&CK, threat hunting, análisis de incidentes y perfiles de grupos adversarios.

**¿Por qué me afecta?**  
El análisis de TTP permite centrarse en el comportamiento del atacante en lugar de depender únicamente de indicadores que pueden cambiar fácilmente.

**¿Cómo se soluciona?**  
Identificando TTP relevantes, creando detecciones basadas en comportamiento y utilizando esa información para fortalecer controles y capacidades de threat hunting.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede adaptar sus herramientas e indicadores mientras mantiene TTP similares, dificultando su detección si las defensas dependen exclusivamente de firmas o IOCs.
