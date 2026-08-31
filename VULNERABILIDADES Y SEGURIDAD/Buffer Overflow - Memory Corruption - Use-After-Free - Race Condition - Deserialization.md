# Buffer Overflow

**¿Qué es?**  
Buffer Overflow es una vulnerabilidad que ocurre cuando un programa escribe más datos de los que un área de memoria reservada puede almacenar, provocando que los datos sobrescriban memoria adyacente.

**¿Dónde lo encuentro?**  
En software desarrollado con lenguajes que permiten una gestión manual de memoria, sistemas operativos, aplicaciones, librerías y dispositivos.

**¿Por qué me afecta?**  
Puede provocar fallos del programa, corrupción de memoria y, en determinadas condiciones, permitir la ejecución de código no autorizado.

**¿Cómo se soluciona?**  
Validando correctamente los tamaños de entrada, utilizando funciones seguras, aplicando protecciones de memoria y manteniendo actualizado el software vulnerable.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede proporcionar datos especialmente diseñados para sobrescribir memoria y alterar el comportamiento de un programa vulnerable.

---

# Memory Corruption

**¿Qué es?**  
Memory Corruption es una condición en la que un programa modifica una región de memoria de forma incorrecta, provocando que los datos almacenados o utilizados por el programa queden alterados.

**¿Dónde lo encuentro?**  
En software que realiza gestión manual de memoria, sistemas operativos, aplicaciones, librerías y controladores.

**¿Por qué me afecta?**  
Puede provocar crashes, comportamiento inesperado, pérdida de integridad de datos o, en ciertos casos, ejecución de código.

**¿Cómo se soluciona?**  
Utilizando prácticas seguras de gestión de memoria, validando límites, realizando análisis de código y aplicando actualizaciones de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede buscar una operación que permita corromper memoria y manipular el comportamiento del proceso afectado.

---

# Use-After-Free

**¿Qué es?**  
Use-After-Free es una vulnerabilidad que ocurre cuando un programa continúa utilizando una región de memoria después de haberla liberado.

**¿Dónde lo encuentro?**  
En aplicaciones y librerías que gestionan memoria manualmente, especialmente software de bajo nivel y componentes complejos.

**¿Por qué me afecta?**  
Puede provocar corrupción de memoria, fallos de la aplicación y, dependiendo de las condiciones, ejecución de código no autorizado.

**¿Cómo se soluciona?**  
Gestionando correctamente el ciclo de vida de los objetos, evitando referencias a memoria liberada y utilizando herramientas de análisis y detección de errores de memoria.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar provocar que el programa utilice memoria que ya fue liberada y manipular el estado de esa memoria para influir en el comportamiento del proceso.

---

# Race Condition

**¿Qué es?**  
Race Condition es una vulnerabilidad que ocurre cuando el resultado de una operación depende del orden o momento en que diferentes procesos o hilos acceden o modifican un recurso compartido.

**¿Dónde lo encuentro?**  
En aplicaciones concurrentes, sistemas operativos, servicios, APIs, sistemas de archivos y aplicaciones que manejan recursos compartidos.

**¿Por qué me afecta?**  
Puede provocar inconsistencias, acceso no autorizado, corrupción de datos o permitir que una operación de seguridad sea evitada debido a una condición temporal.

**¿Cómo se soluciona?**  
Utilizando mecanismos adecuados de sincronización, operaciones atómicas, controles de acceso consistentes y evitando depender de comprobaciones separadas de la operación que protegen.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar ejecutar acciones simultáneas o en una ventana de tiempo específica para aprovechar la diferencia entre una comprobación y la operación posterior.

---

# Deserialization

**¿Qué es?**  
Deserialization es el proceso mediante el cual datos almacenados o transmitidos en un formato serializado se convierten nuevamente en objetos o estructuras que una aplicación puede utilizar.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, sistemas distribuidos, aplicaciones empresariales y servicios que intercambian objetos o estructuras de datos.

**¿Por qué me afecta?**  
Una deserialización insegura puede permitir manipulación de objetos, ejecución de acciones no deseadas o, en determinadas tecnologías, ejecución remota de código.

**¿Cómo se soluciona?**  
Evitando deserializar datos no confiables cuando sea posible, utilizando formatos seguros, validando estrictamente los datos y restringiendo los tipos de objetos permitidos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede modificar datos serializados para intentar alterar el comportamiento de la aplicación durante el proceso de deserialización.
