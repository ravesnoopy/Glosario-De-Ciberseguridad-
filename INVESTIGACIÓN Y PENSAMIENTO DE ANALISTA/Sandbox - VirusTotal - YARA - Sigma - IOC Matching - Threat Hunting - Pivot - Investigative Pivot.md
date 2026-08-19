
## Sandbox

**¿Qué es?**  
Un Sandbox es un entorno aislado utilizado para ejecutar o analizar archivos, aplicaciones o comportamientos sospechosos sin exponer directamente el sistema de producción.

**¿Dónde lo encuentro?**  
En plataformas de análisis de malware, laboratorios de seguridad, soluciones EDR y entornos utilizados por equipos SOC y DFIR.

**¿Por qué me afecta?**  
Permite observar el comportamiento de contenido potencialmente malicioso y obtener evidencia sin ejecutarlo directamente en un entorno crítico.

**¿Cómo se soluciona?**  
Utilizando entornos aislados, controlando la conectividad, registrando la actividad y evitando que el sandbox tenga acceso innecesario a sistemas reales.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede detectar que está siendo ejecutado en un entorno de análisis y modificar o retrasar su comportamiento para evitar revelar sus acciones maliciosas.

## VirusTotal

**¿Qué es?**  
VirusTotal es un servicio de análisis que permite consultar archivos, URLs, dominios, direcciones IP y otros indicadores utilizando múltiples fuentes de seguridad y motores de detección.

**¿Dónde lo encuentro?**  
En investigaciones de malware, análisis de archivos, validación de indicadores y actividades de threat intelligence.

**¿Por qué me afecta?**  
Puede ayudar a determinar si un indicador es conocido como malicioso y aportar contexto útil durante una investigación.

**¿Cómo se soluciona?**  
Consultando indicadores relevantes, comparando resultados de múltiples fuentes y validando los hallazgos con evidencia adicional antes de tomar decisiones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar archivos o infraestructura para evitar coincidencias con indicadores conocidos y reducir la probabilidad de detección.

## YARA

**¿Qué es?**  
YARA es una herramienta y lenguaje de reglas utilizado para identificar y clasificar archivos o patrones asociados con malware y otras características relevantes.

**¿Dónde lo encuentro?**  
En análisis de malware, threat hunting, DFIR y sistemas utilizados para identificar familias o artefactos específicos.

**¿Por qué me afecta?**  
Permite detectar archivos que comparten características conocidas con amenazas, incluso cuando no existe una firma antivirus tradicional.

**¿Cómo se soluciona?**  
Desarrollando reglas precisas, validándolas contra muestras conocidas y actualizándolas cuando aparecen nuevas variantes.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar características identificables de su malware para evitar coincidir con reglas YARA conocidas.

## Sigma

**¿Qué es?**  
Sigma es un formato abierto y genérico para describir reglas de detección basadas principalmente en registros de eventos, permitiendo adaptar una misma lógica a diferentes plataformas SIEM.

**¿Dónde lo encuentro?**  
En threat hunting, detección de amenazas, SOC y repositorios de reglas utilizadas para analizar logs.

**¿Por qué me afecta?**  
Permite crear detecciones reutilizables y compartir lógica de detección independientemente de un SIEM específico.

**¿Cómo se soluciona?**  
Creando reglas basadas en comportamientos relevantes, validándolas con datos reales y convirtiéndolas al formato requerido por la plataforma utilizada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar modificar su comportamiento para evitar los patrones de eventos que las reglas de detección buscan identificar.

## IOC Matching

**¿Qué es?**  
IOC Matching es el proceso de comparar datos observados en un entorno con Indicadores de Compromiso (IOCs) conocidos, como hashes, dominios, direcciones IP o nombres de archivos.

**¿Dónde lo encuentro?**  
En SIEM, EDR, plataformas de threat intelligence, herramientas de monitoreo y procesos de investigación de incidentes.

**¿Por qué me afecta?**  
Permite identificar rápidamente posibles relaciones entre la actividad observada y amenazas previamente conocidas.

**¿Cómo se soluciona?**  
Manteniendo fuentes confiables de inteligencia, realizando coincidencias sobre logs y endpoints y validando los resultados con contexto adicional.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede cambiar sus indicadores, utilizar infraestructura nueva o modificar archivos para evitar coincidencias directas.

## Threat Hunting

**¿Qué es?**  
Threat Hunting es la búsqueda proactiva y estructurada de actividad potencialmente maliciosa que puede no haber generado una alerta automática.

**¿Dónde lo encuentro?**  
En SOC, equipos de detección y respuesta, EDR, SIEM, análisis de red y procesos de threat intelligence.

**¿Por qué me afecta?**  
Permite descubrir amenazas que evadieron controles automáticos y encontrar comportamientos sospechosos antes de que produzcan un impacto mayor.

**¿Cómo se soluciona?**  
Formulando hipótesis, analizando telemetría, buscando patrones anómalos y refinando las detecciones a partir de los hallazgos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar técnicas de evasión, herramientas legítimas y comportamientos similares a los de usuarios normales para dificultar su descubrimiento.

## Pivot

**¿Qué es?**  
Pivot es el cambio de un punto de análisis, fuente de información o indicador hacia otro elemento relacionado para ampliar una investigación.

**¿Dónde lo encuentro?**  
En threat hunting, DFIR, análisis de malware, threat intelligence e investigaciones de incidentes.

**¿Por qué me afecta?**  
Permite pasar de una evidencia conocida a otras entidades relacionadas y descubrir conexiones que inicialmente no eran visibles.

**¿Cómo se soluciona?**  
Utilizando relaciones entre indicadores, usuarios, hosts, procesos, dominios, direcciones IP y eventos para ampliar progresivamente la investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Un atacante puede utilizar múltiples sistemas, cuentas o indicadores relacionados para distribuir sus actividades y dificultar la identificación de toda la infraestructura comprometida.

## Investigative Pivot

**¿Qué es?**  
Investigative Pivot es el cambio deliberado de una línea de investigación hacia otra evidencia o fuente relacionada después de encontrar información que puede revelar nuevas conexiones relevantes.

**¿Dónde lo encuentro?**  
En investigaciones DFIR, threat hunting, análisis de incidentes y análisis de inteligencia de amenazas.

**¿Por qué me afecta?**  
Permite adaptar la investigación a nuevos hallazgos y evitar que el análisis quede limitado a la evidencia inicialmente identificada.

**¿Cómo se soluciona?**  
Partiendo de un indicador o hallazgo, identificando relaciones relevantes y siguiendo esas conexiones mediante nuevas consultas, fuentes o evidencias.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede distribuir su actividad entre múltiples cuentas, dispositivos, dominios o técnicas para dificultar que una investigación conecte todos los elementos relacionados.
