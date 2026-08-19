
## Behavioral Detection

**¿Qué es?**  
Behavioral Detection identifica actividades sospechosas mediante patrones de comportamiento, en lugar de depender únicamente de firmas conocidas.

**¿Dónde lo encuentro?**  
En EDR, SIEM, NDR, sistemas de detección y plataformas de seguridad que analizan el comportamiento de usuarios, procesos o dispositivos.

**¿Por qué me afecta?**  
Puede detectar amenazas nuevas o variantes que no tienen una firma conocida, especialmente cuando presentan comportamientos anómalos.

**¿Cómo se soluciona?**  
Definiendo comportamientos esperados, creando reglas de detección y ajustándolas continuamente para reducir falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar imitar comportamientos legítimos, utilizar herramientas nativas del sistema o modificar su actividad para evitar patrones de detección.

## Signature Detection

**¿Qué es?**  
Signature Detection identifica amenazas comparando archivos, tráfico o eventos con patrones previamente conocidos de actividad maliciosa.

**¿Dónde lo encuentro?**  
En antivirus, IDS, IPS, EDR, SIEM y otras herramientas de seguridad.

**¿Por qué me afecta?**  
Es eficaz para detectar amenazas conocidas, pero puede no identificar malware nuevo o técnicas modificadas que no coincidan con una firma existente.

**¿Cómo se soluciona?**  
Manteniendo actualizadas las firmas y combinando esta detección con análisis de comportamiento y otras técnicas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar malware, cambiar indicadores conocidos o utilizar herramientas legítimas para evitar coincidir con firmas existentes.

## Anomaly Detection

**¿Qué es?**  
Anomaly Detection identifica actividades que se desvían significativamente del comportamiento considerado normal para un usuario, sistema o entorno.

**¿Dónde lo encuentro?**  
En SIEM, EDR, NDR, sistemas de análisis de comportamiento y plataformas de seguridad.

**¿Por qué me afecta?**  
Puede revelar actividades que no coinciden con los patrones habituales, incluso cuando no existe una firma específica para la amenaza.

**¿Cómo se soluciona?**  
Definiendo modelos o reglas de comportamiento normal y revisando continuamente las anomalías detectadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede mantener una actividad de bajo volumen y similar al comportamiento legítimo para reducir la probabilidad de ser identificado como una anomalía.

## Baseline

**¿Qué es?**  
Baseline es una referencia del comportamiento, configuración o actividad considerada normal para un sistema, usuario o entorno.

**¿Dónde lo encuentro?**  
En monitoreo de endpoints, redes, SIEM, gestión de configuración y análisis de comportamiento.

**¿Por qué me afecta?**  
Permite comparar la actividad actual con un comportamiento esperado y detectar desviaciones potencialmente sospechosas.

**¿Cómo se soluciona?**  
Estableciendo baselines actualizados y revisándolos cuando cambian los sistemas, usuarios o procesos legítimos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar permanecer dentro de patrones aparentemente normales para evitar generar desviaciones detectables.

## Threat Hunting

**¿Qué es?**  
Threat Hunting es la búsqueda proactiva y dirigida de amenazas que podrían no haber generado una alerta automática.

**¿Dónde lo encuentro?**  
En equipos SOC, plataformas SIEM, EDR, NDR, repositorios de logs y herramientas de análisis de amenazas.

**¿Por qué me afecta?**  
Permite descubrir actividad maliciosa que los controles automatizados no detectaron y validar posibles hipótesis de compromiso.

**¿Cómo se soluciona?**  
Definiendo hipótesis, consultando datos relevantes, buscando patrones sospechosos y documentando los resultados de cada investigación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede minimizar indicadores, utilizar herramientas legítimas y mantener comportamientos discretos para dificultar una búsqueda proactiva.

## Hypothesis

**¿Qué es?**  
Hypothesis es una suposición fundamentada sobre una posible actividad maliciosa que guía una investigación de Threat Hunting.

**¿Dónde lo encuentro?**  
En procesos de Threat Hunting, investigaciones SOC, análisis de incidentes y ejercicios de detección.

**¿Por qué me afecta?**  
Una hipótesis bien definida ayuda a enfocar la búsqueda y evita analizar grandes cantidades de datos sin un objetivo claro.

**¿Cómo se soluciona?**  
Formulando hipótesis basadas en amenazas, comportamientos observables y contexto del entorno, y validándolas mediante evidencia.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar técnicas poco comunes o cambiar su comportamiento para que una hipótesis específica no encuentre evidencia suficiente.

## Hunt Query

**¿Qué es?**  
Hunt Query es una consulta diseñada para buscar indicadores, comportamientos o patrones específicos dentro de grandes conjuntos de datos de seguridad.

**¿Dónde lo encuentro?**  
En SIEM, EDR, plataformas de Threat Hunting, bases de datos de logs y herramientas de análisis.

**¿Por qué me afecta?**  
Permite buscar evidencia de actividad maliciosa de forma sistemática y validar hipótesis durante una investigación.

**¿Cómo se soluciona?**  
Construyendo consultas precisas, utilizando los campos disponibles y refinándolas para equilibrar cobertura y falsos positivos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar indicadores o utilizar variaciones de una técnica para evitar coincidir con consultas demasiado específicas.
