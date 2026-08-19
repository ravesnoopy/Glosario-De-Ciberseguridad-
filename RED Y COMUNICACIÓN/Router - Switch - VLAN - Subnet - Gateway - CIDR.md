
## Router

**¿Qué es?**  
Dispositivo de red que conecta diferentes redes y determina hacia dónde debe enviarse el tráfico IP.

**¿Dónde lo encuentro?**  
En redes domésticas, empresariales, centros de datos, proveedores de Internet y entornos cloud.

**¿Por qué me afecta?**  
Controla el flujo de tráfico entre redes y puede ser un punto crítico para segmentación, filtrado y seguridad perimetral.

**¿Cómo se soluciona?**  
Mantener el firmware actualizado, restringir la administración, aplicar reglas de filtrado y revisar periódicamente su configuración.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentaría comprometerlo o aprovechar una configuración débil para interceptar, redirigir o controlar el tráfico entre redes.


## Switch

**¿Qué es?**  
Dispositivo de red que conecta equipos dentro de una red local y reenvía tramas hacia el puerto correspondiente.

**¿Dónde lo encuentro?**  
En redes empresariales, centros de datos, oficinas y redes domésticas.

**¿Por qué me afecta?**  
Una configuración insegura puede facilitar accesos no autorizados o afectar la segmentación y comunicación dentro de la red local.

**¿Cómo se soluciona?**  
Aplicar VLAN, controles de acceso, deshabilitar puertos no utilizados y proteger las interfaces de administración.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar aprovechar configuraciones débiles del switch para obtener acceso a segmentos o interceptar tráfico de la red local.


## VLAN

**¿Qué es?**  
Virtual Local Area Network permite dividir lógicamente una red física en diferentes segmentos de red.

**¿Dónde lo encuentro?**  
En switches administrables, redes empresariales, centros de datos y entornos donde se requiere segmentación.

**¿Por qué me afecta?**  
Una segmentación incorrecta puede permitir que un dispositivo acceda a recursos que deberían estar aislados.

**¿Cómo se soluciona?**  
Definir correctamente las VLAN, controlar el tráfico entre segmentos y proteger las configuraciones de puertos y enlaces.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar aprovechar errores de configuración para acceder a tráfico o recursos pertenecientes a otra VLAN.


## Subnet

**¿Qué es?**  
Segmento lógico de una red IP que permite dividir un espacio de direcciones en redes más pequeñas.

**¿Dónde lo encuentro?**  
En redes corporativas, domésticas, centros de datos, dispositivos de red y entornos cloud.

**¿Por qué me afecta?**  
Una correcta división en subredes ayuda a limitar comunicaciones y reducir la superficie de exposición entre sistemas.

**¿Cómo se soluciona?**  
Diseñar subredes según las necesidades de seguridad y aplicar controles de acceso entre ellas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar una segmentación deficiente para desplazarse desde un sistema comprometido hacia otros recursos de la misma red.


## Gateway

**¿Qué es?**  
Dispositivo o dirección que sirve como punto de salida de una red y permite que los sistemas se comuniquen con otras redes.

**¿Dónde lo encuentro?**  
En configuraciones de dispositivos, routers, redes empresariales, redes domésticas y entornos cloud.

**¿Por qué me afecta?**  
Un gateway comprometido o mal configurado puede permitir redirección, interceptación o bloqueo del tráfico.

**¿Cómo se soluciona?**  
Proteger el dispositivo, restringir su administración, aplicar reglas de filtrado y mantener una configuración segura.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría intentar comprometerlo para manipular el tráfico, bloquear comunicaciones o redirigir dispositivos hacia recursos controlados por él.


## CIDR

**¿Qué es?**  
Classless Inter-Domain Routing es un método para representar y asignar bloques de direcciones IP mediante una longitud de prefijo, como `192.168.1.0/24`.

**¿Dónde lo encuentro?**  
En configuraciones de redes, routers, firewalls, tablas de enrutamiento y servicios cloud.

**¿Por qué me afecta?**  
Una definición incorrecta de los rangos puede provocar exposición innecesaria, problemas de enrutamiento o acceso entre redes que deberían estar separadas.

**¿Cómo se soluciona?**  
Planificar correctamente los rangos CIDR y revisar las reglas de enrutamiento y acceso asociadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Podría aprovechar rangos demasiado amplios o reglas mal configuradas para alcanzar sistemas que no deberían estar accesibles desde su posición.
