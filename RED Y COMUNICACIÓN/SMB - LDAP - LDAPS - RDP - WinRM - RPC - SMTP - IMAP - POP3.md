
## SMB

**¿Qué es?**  
SMB (Server Message Block) es un protocolo utilizado para compartir archivos, impresoras y otros recursos de red, especialmente en entornos Windows.

**¿Dónde lo encuentro?**  
En servidores de archivos, recursos compartidos, Windows y redes empresariales, normalmente mediante puertos como `445`.

**¿Por qué me afecta?**  
Una configuración insegura de SMB puede exponer archivos, credenciales o servicios y facilitar movimientos laterales dentro de una red.

**¿Cómo se soluciona?**  
Deshabilitando versiones inseguras, restringiendo el acceso, aplicando autenticación adecuada y monitoreando conexiones SMB sospechosas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar SMB para acceder a recursos compartidos, obtener información, ejecutar acciones remotas o desplazarse hacia otros sistemas.

## LDAP

**¿Qué es?**  
LDAP (Lightweight Directory Access Protocol) es un protocolo utilizado para consultar y administrar información almacenada en servicios de directorio.

**¿Dónde lo encuentro?**  
En servicios de directorio como Active Directory, servidores LDAP y aplicaciones que consultan información de usuarios, grupos y recursos.

**¿Por qué me afecta?**  
Las consultas LDAP pueden revelar información sobre usuarios, grupos, equipos y relaciones dentro de una organización.

**¿Cómo se soluciona?**  
Aplicando controles de acceso, mínimo privilegio, autenticación segura y monitoreando consultas LDAP anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede realizar consultas LDAP para enumerar usuarios, grupos, equipos y otra información útil para planificar movimientos dentro del entorno.

## LDAPS

**¿Qué es?**  
LDAPS (LDAP over SSL/TLS) es LDAP protegido mediante TLS para cifrar la comunicación entre el cliente y el servidor de directorio.

**¿Dónde lo encuentro?**  
En Active Directory y otros servicios de directorio configurados para proteger las comunicaciones LDAP mediante TLS.

**¿Por qué me afecta?**  
Sin protección adecuada, las consultas y credenciales transmitidas mediante LDAP pueden quedar expuestas a interceptación.

**¿Cómo se soluciona?**  
Utilizando TLS correctamente configurado, certificados válidos y configuraciones que eviten protocolos o métodos de autenticación inseguros.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar interceptar comunicaciones LDAP cuando no están adecuadamente protegidas o aprovechar configuraciones TLS débiles.

## RDP

**¿Qué es?**  
RDP (Remote Desktop Protocol) es un protocolo que permite acceder remotamente a la interfaz gráfica de un sistema Windows.

**¿Dónde lo encuentro?**  
En servidores y estaciones Windows que permiten administración o acceso remoto, normalmente mediante el puerto `3389`.

**¿Por qué me afecta?**  
Un RDP expuesto o mal protegido puede convertirse en un punto de entrada para ataques de credenciales y acceso remoto no autorizado.

**¿Cómo se soluciona?**  
Restringiendo el acceso mediante VPN o controles de red, utilizando MFA cuando sea posible, aplicando parches y monitoreando autenticaciones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar obtener o reutilizar credenciales para acceder remotamente a sistemas mediante RDP y continuar el ataque desde ellos.

## WinRM

**¿Qué es?**  
WinRM (Windows Remote Management) es un servicio de Windows que permite administrar sistemas remotamente mediante WS-Management.

**¿Dónde lo encuentro?**  
En sistemas Windows y entornos empresariales donde se utilizan herramientas de administración remota y automatización.

**¿Por qué me afecta?**  
Un WinRM accesible y con controles débiles puede proporcionar capacidades de administración remota que un atacante podría aprovechar.

**¿Cómo se soluciona?**  
Restringiendo el acceso a administradores autorizados, utilizando autenticación segura, segmentación de red y monitoreo de conexiones remotas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales comprometidas y WinRM para ejecutar acciones remotamente o desplazarse hacia otros sistemas.

## RPC

**¿Qué es?**  
RPC (Remote Procedure Call) es un mecanismo que permite que un programa solicite la ejecución de funciones o procedimientos en otro proceso o sistema.

**¿Dónde lo encuentro?**  
En sistemas Windows, aplicaciones distribuidas, servicios de red y mecanismos de administración remota.

**¿Por qué me afecta?**  
Algunos servicios RPC pueden exponer funciones administrativas o vulnerabilidades que permitan acceso o ejecución remota.

**¿Cómo se soluciona?**  
Restringiendo servicios y puertos RPC, aplicando parches, utilizando segmentación y monitoreando conexiones y actividades anómalas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede aprovechar servicios RPC vulnerables o accesibles para ejecutar acciones remotamente o desplazarse dentro de la red.

## SMTP

**¿Qué es?**  
SMTP (Simple Mail Transfer Protocol) es un protocolo utilizado principalmente para enviar y transferir correo electrónico entre servidores y sistemas de correo.

**¿Dónde lo encuentro?**  
En servidores de correo, gateways, aplicaciones y servicios que envían o reciben mensajes electrónicos.

**¿Por qué me afecta?**  
Un servidor SMTP mal configurado puede facilitar spam, abuso de cuentas o ataques relacionados con correo electrónico.

**¿Cómo se soluciona?**  
Configurando autenticación, restricciones de relay, protección contra abuso y mecanismos de seguridad para correo electrónico.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede abusar de servidores SMTP para enviar phishing, spam o mensajes que intenten engañar a los usuarios.

## IMAP

**¿Qué es?**  
IMAP (Internet Message Access Protocol) es un protocolo utilizado para acceder y administrar mensajes almacenados en un servidor de correo.

**¿Dónde lo encuentro?**  
En clientes de correo electrónico y servidores que permiten consultar buzones remotamente.

**¿Por qué me afecta?**  
Una cuenta IMAP comprometida puede proporcionar acceso a correos que contienen información sensible, enlaces, documentos o credenciales.

**¿Cómo se soluciona?**  
Utilizando TLS, MFA cuando esté disponible, contraseñas robustas y monitoreando accesos anómalos a los buzones.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede utilizar credenciales robadas para acceder a buzones y recopilar información útil para continuar una intrusión.

## POP3

**¿Qué es?**  
POP3 (Post Office Protocol version 3) es un protocolo utilizado para descargar mensajes de correo electrónico desde un servidor hacia un cliente.

**¿Dónde lo encuentro?**  
En clientes y servidores de correo que utilizan POP3 para la recuperación de mensajes.

**¿Por qué me afecta?**  
Una configuración insegura puede exponer credenciales o permitir acceso no autorizado a buzones y mensajes.

**¿Cómo se soluciona?**  
Utilizando versiones protegidas mediante TLS, autenticación segura y restringiendo POP3 cuando no sea necesario.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar utilizar credenciales comprometidas para acceder a buzones y obtener información que facilite otras etapas del ataque.
