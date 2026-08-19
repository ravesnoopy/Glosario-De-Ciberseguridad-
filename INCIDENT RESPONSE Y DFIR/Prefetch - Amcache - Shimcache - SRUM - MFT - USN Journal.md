
## Prefetch

**¿Qué es?**  
Artefacto de Windows que registra información relacionada con la ejecución de aplicaciones para ayudar a optimizar su carga y rendimiento.

**¿Dónde lo encuentro?**  
Principalmente en `C:\Windows\Prefetch\`, donde se almacenan archivos `.pf` asociados con aplicaciones ejecutadas.

**¿Por qué me afecta?**  
Puede proporcionar evidencia de ejecución de programas y ayudar a determinar qué aplicaciones fueron utilizadas en un sistema durante una investigación.

**¿Cómo se soluciona?**  
No requiere una corrección específica; desde el punto de vista forense, debe preservarse y analizarse junto con otros artefactos para validar la actividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría eliminar o manipular artefactos de ejecución para dificultar que los investigadores determinen qué programas fueron ejecutados.


## Amcache

**¿Qué es?**  
Artefacto de Windows que almacena información sobre aplicaciones y archivos ejecutables observados por el sistema, proporcionando evidencia útil sobre software presente o ejecutado.

**¿Dónde lo encuentro?**  
Principalmente en la estructura de registro de Windows, especialmente en `C:\Windows\AppCompat\Programs\Amcache.hve`.

**¿Por qué me afecta?**  
Puede ayudar a identificar ejecutables, rutas, información de archivos y actividad relacionada con software durante una investigación forense.

**¿Cómo se soluciona?**  
No requiere una corrección específica; debe preservarse la evidencia y analizarse considerando que su presencia no demuestra por sí sola que un archivo haya sido ejecutado.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar eliminar o manipular evidencias del sistema para dificultar la identificación de herramientas o ejecutables utilizados.


## Shimcache

**¿Qué es?**  
Artefacto de compatibilidad de Windows que mantiene información utilizada por el sistema para gestionar problemas de compatibilidad de aplicaciones y que puede aportar evidencia forense.

**¿Dónde lo encuentro?**  
En estructuras del registro de Windows relacionadas con `AppCompatCache`, almacenadas en el hive `SYSTEM`.

**¿Por qué me afecta?**  
Puede proporcionar información útil para investigar la presencia de determinados ejecutables, aunque su evidencia no debe interpretarse automáticamente como prueba de ejecución.

**¿Cómo se soluciona?**  
No requiere una corrección específica; debe analizarse junto con otros artefactos y eventos para establecer si realmente ocurrió una ejecución.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría eliminar o manipular evidencias relacionadas con sus herramientas para dificultar la reconstrucción de sus actividades.


## SRUM

**¿Qué es?**  
System Resource Usage Monitor es un componente de Windows que registra información sobre el uso de recursos y actividad de aplicaciones y procesos.

**¿Dónde lo encuentro?**  
Principalmente en la base de datos `SRUDB.dat`, ubicada normalmente en `C:\Windows\System32\sru\`.

**¿Por qué me afecta?**  
Puede aportar información sobre actividad de aplicaciones, consumo de recursos y comunicaciones de red, ayudando a reconstruir acciones ocurridas en un sistema.

**¿Cómo se soluciona?**  
No requiere una corrección específica; debe conservarse y analizarse como parte de la evidencia forense disponible.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría borrar o manipular registros y artefactos que permitan relacionar una aplicación con actividad realizada durante el compromiso.


## MFT

**¿Qué es?**  
Master File Table es una estructura fundamental del sistema de archivos NTFS que contiene registros e información sobre archivos y directorios almacenados en un volumen.

**¿Dónde lo encuentro?**  
En volúmenes formateados con NTFS, donde forma parte de las estructuras internas del sistema de archivos.

**¿Por qué me afecta?**  
Puede proporcionar información sobre archivos, rutas, tamaños y marcas temporales, siendo una fuente importante para investigaciones forenses de disco.

**¿Cómo se soluciona?**  
No requiere una corrección; durante una investigación debe preservarse la evidencia del sistema de archivos y analizarse mediante técnicas forenses adecuadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar eliminar archivos o manipular información asociada para dificultar la reconstrucción de sus actividades.


## USN Journal

**¿Qué es?**  
Registro de NTFS que mantiene información sobre cambios realizados en archivos y directorios, como creación, modificación, eliminación o renombrado.

**¿Dónde lo encuentro?**  
En volúmenes NTFS, dentro de la estructura `$Extend\$UsnJrnl`.

**¿Por qué me afecta?**  
Puede ayudar a reconstruir cambios realizados en el sistema de archivos incluso cuando determinados archivos ya no están presentes.

**¿Cómo se soluciona?**  
No requiere una corrección específica; debe preservarse y correlacionarse con otros artefactos para determinar qué cambios ocurrieron y cuándo.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría eliminar o manipular evidencias relacionadas con archivos creados, modificados o eliminados para dificultar el análisis forense.
