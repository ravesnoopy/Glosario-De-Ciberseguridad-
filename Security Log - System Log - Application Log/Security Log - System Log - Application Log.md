
## Security Log

**¿Qué es?**  
Security Log es un registro de eventos relacionados con la seguridad de un sistema, como autenticaciones, uso de privilegios y cambios relevantes.

**¿Dónde lo encuentro?**  
En sistemas Windows, especialmente en servidores y estaciones de trabajo donde está habilitada la auditoría de seguridad.

**¿Por qué me afecta?**  
Proporciona evidencia sobre accesos exitosos o fallidos, uso de cuentas y otras actividades que pueden indicar compromiso o abuso de privilegios.

**¿Cómo se soluciona?**  
Habilitando una política de auditoría adecuada, centralizando los registros y protegiéndolos contra modificaciones o eliminación no autorizada.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar borrar eventos, modificar configuraciones de auditoría o evitar generar registros para dificultar la investigación.

## System Log

**¿Qué es?**  
System Log es un registro que contiene eventos relacionados con el funcionamiento del sistema operativo y sus componentes.

**¿Dónde lo encuentro?**  
En sistemas operativos, servidores y estaciones de trabajo, incluyendo los registros centralizados en un SIEM.

**¿Por qué me afecta?**  
Puede revelar cambios en servicios, errores, fallos de componentes y otras actividades que ayuden a identificar comportamientos anómalos.

**¿Cómo se soluciona?**  
Recopilando los eventos relevantes, protegiendo los registros y correlacionándolos con otras fuentes de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede manipular servicios o componentes del sistema y posteriormente intentar eliminar los registros que evidencien sus acciones.

## Application Log

**¿Qué es?**  
Application Log es un registro que contiene eventos generados por aplicaciones y servicios, como errores, advertencias y otras actividades relevantes.

**¿Dónde lo encuentro?**  
En sistemas operativos, servidores y aplicaciones que mantienen registros de sus propias operaciones.

**¿Por qué me afecta?**  
Puede proporcionar evidencia de errores, accesos, fallos o comportamientos anómalos dentro de una aplicación comprometida.

**¿Cómo se soluciona?**  
Habilitando los registros necesarios, centralizándolos y estableciendo políticas adecuadas de protección y retención.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede explotar una vulnerabilidad de una aplicación y posteriormente intentar borrar o modificar sus registros para ocultar la actividad realizada.
