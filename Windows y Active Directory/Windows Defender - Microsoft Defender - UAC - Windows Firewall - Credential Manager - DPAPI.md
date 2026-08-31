# Windows Defender

**¿Qué es?**  
Windows Defender es el conjunto de capacidades de seguridad integrado en Windows que ayuda a proteger el sistema frente a malware, amenazas y actividades sospechosas.

**¿Dónde lo encuentro?**  
En sistemas Windows, donde proporciona diferentes funciones de protección, detección y seguridad del endpoint.

**¿Por qué me afecta?**  
Ayuda a prevenir y detectar amenazas que podrían comprometer el equipo, sus datos y las credenciales almacenadas.

**¿Cómo se soluciona?**  
Manteniendo actualizadas sus capacidades de protección, aplicando políticas de seguridad adecuadas y verificando que los mecanismos de protección estén activos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evadir, deshabilitar o degradar las protecciones de Defender después de obtener los permisos necesarios.

---

# Microsoft Defender

**¿Qué es?**  
Microsoft Defender es la plataforma de seguridad de Microsoft que proporciona diferentes capacidades de prevención, detección, investigación y respuesta frente a amenazas.

**¿Dónde lo encuentro?**  
En el ecosistema Microsoft, incluyendo dispositivos Windows, servidores, identidades, aplicaciones y servicios cloud según la solución implementada.

**¿Por qué me afecta?**  
Proporciona capacidades de seguridad que ayudan a detectar y responder ante actividades maliciosas en diferentes componentes del entorno.

**¿Cómo se soluciona?**  
Configurando correctamente las políticas, manteniendo los componentes actualizados y monitoreando las alertas y recomendaciones de seguridad.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar evadir las capacidades de detección, desactivar controles o aprovechar configuraciones débiles para evitar ser detectado.

---

# UAC

**¿Qué es?**  
UAC (User Account Control) es una función de Windows que ayuda a impedir que cambios que requieren privilegios administrativos se realicen silenciosamente.

**¿Dónde lo encuentro?**  
En sistemas Windows, como parte del mecanismo de control de privilegios del sistema operativo.

**¿Por qué me afecta?**  
Ayuda a limitar las acciones administrativas realizadas por procesos que se ejecutan con un nivel de privilegio inferior.

**¿Cómo se soluciona?**  
Manteniendo UAC habilitado y configurando adecuadamente sus niveles de notificación y políticas relacionadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar encontrar formas de ejecutar acciones con privilegios elevados sin generar la interacción esperada del usuario.

---

# Windows Firewall

**¿Qué es?**  
Windows Firewall es el firewall integrado de Windows que controla las conexiones de red según reglas que permiten o bloquean determinado tráfico.

**¿Dónde lo encuentro?**  
En equipos y servidores Windows mediante Windows Defender Firewall y sus herramientas de administración.

**¿Por qué me afecta?**  
Una configuración adecuada puede impedir conexiones no autorizadas y reducir la exposición de servicios.

**¿Cómo se soluciona?**  
Aplicando reglas basadas en mínimo privilegio, permitiendo únicamente el tráfico necesario y revisando periódicamente las reglas configuradas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar reglas demasiado permisivas o intentar modificar la configuración del firewall si obtiene privilegios suficientes.

---

# Credential Manager

**¿Qué es?**  
Credential Manager es una función de Windows que permite almacenar y administrar determinadas credenciales utilizadas para acceder a recursos, aplicaciones y servicios.

**¿Dónde lo encuentro?**  
En sistemas Windows, mediante la configuración de cuentas y las herramientas de administración de credenciales.

**¿Por qué me afecta?**  
Las credenciales almacenadas pueden proporcionar acceso a recursos adicionales si son obtenidas por una persona o proceso no autorizado.

**¿Cómo se soluciona?**  
Evitando almacenar credenciales innecesariamente, protegiendo las cuentas, aplicando mínimo privilegio y monitoreando accesos sospechosos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar acceder a credenciales almacenadas para reutilizarlas y obtener acceso a otros recursos.

---

# DPAPI

**¿Qué es?**  
DPAPI (Data Protection API) es un mecanismo de Windows que permite proteger datos sensibles mediante claves vinculadas al usuario o al sistema.

**¿Dónde lo encuentro?**  
En sistemas Windows y aplicaciones que utilizan las capacidades de protección de datos proporcionadas por el sistema operativo.

**¿Por qué me afecta?**  
DPAPI puede proteger información sensible utilizada por aplicaciones y usuarios. Si las claves o el contexto necesario para descifrarla son comprometidos, los datos protegidos también pueden quedar en riesgo.

**¿Cómo se soluciona?**  
Protegiendo las cuentas y sistemas que utilizan DPAPI, aplicando mínimo privilegio y monitoreando accesos anómalos a material protegido.

**¿Cómo lo usaría un atacante en mi contra?**  
Después de comprometer una cuenta o sistema, puede intentar acceder al material protegido mediante DPAPI para recuperar información sensible que pueda ser utilizada para acceder a otros recursos.
