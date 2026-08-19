
## OAuth

**¿Qué es?**  
OAuth es un protocolo de autorización que permite a una aplicación acceder a recursos de un usuario en otro servicio sin necesidad de conocer directamente su contraseña.

**¿Dónde lo encuentro?**  
En aplicaciones web, APIs, aplicaciones móviles y servicios que permiten delegar acceso mediante tokens.

**¿Por qué me afecta?**  
Una configuración incorrecta de OAuth puede permitir que un atacante obtenga o abuse de tokens para acceder a recursos sin necesidad de conocer la contraseña del usuario.

**¿Cómo se soluciona?**  
Utilizando flujos adecuados, validando correctamente `redirect_uri`, protegiendo los tokens, aplicando mínimo privilegio y utilizando mecanismos como PKCE cuando corresponda.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar tokens, abusar de aplicaciones OAuth mal configuradas o engañar al usuario para conceder permisos excesivos a una aplicación maliciosa.

## OpenID Connect

**¿Qué es?**  
OpenID Connect (OIDC) es una capa de identidad construida sobre OAuth 2.0 que permite a una aplicación verificar la identidad de un usuario mediante un `ID Token`.

**¿Dónde lo encuentro?**  
En aplicaciones web, aplicaciones móviles y servicios que utilizan proveedores de identidad para implementar inicio de sesión federado.

**¿Por qué me afecta?**  
Una implementación incorrecta puede permitir errores de validación de tokens, suplantación de identidad o acceso no autorizado a cuentas.

**¿Cómo se soluciona?**  
Validando correctamente los tokens, `issuer`, `audience`, firmas y tiempos de expiración, además de proteger adecuadamente los flujos de autenticación.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar manipular o reutilizar tokens, abusar de configuraciones incorrectas o explotar fallos en la validación de la identidad.

## SAML

**¿Qué es?**  
SAML (Security Assertion Markup Language) es un estándar utilizado para intercambiar información de autenticación y autorización entre un proveedor de identidad y un servicio.

**¿Dónde lo encuentro?**  
En aplicaciones empresariales, servicios SaaS y sistemas de Single Sign-On (SSO) utilizados por organizaciones.

**¿Por qué me afecta?**  
Una configuración insegura puede permitir la manipulación o aceptación incorrecta de aserciones y provocar accesos no autorizados.

**¿Cómo se soluciona?**  
Validando firmas y aserciones correctamente, utilizando certificados protegidos, configurando correctamente los proveedores de identidad y servicios, y aplicando controles de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar manipular una aserción SAML, abusar de una configuración incorrecta o comprometer el proveedor de identidad para obtener acceso a aplicaciones federadas.

## MFA

**¿Qué es?**  
MFA (Multi-Factor Authentication) es un mecanismo de autenticación que requiere dos o más factores independientes para verificar la identidad de un usuario.

**¿Dónde lo encuentro?**  
En cuentas corporativas, aplicaciones, VPN, servicios cloud, sistemas administrativos y plataformas que permiten reforzar el inicio de sesión.

**¿Por qué me afecta?**  
Reduce el riesgo de acceso mediante contraseñas robadas, aunque determinados métodos de MFA pueden ser susceptibles a técnicas como phishing o fatiga de autenticación.

**¿Cómo se soluciona?**  
Utilizando métodos resistentes al phishing cuando sea posible, protegiendo los factores de autenticación y aplicando MFA especialmente a cuentas y recursos críticos.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar robar sesiones, engañar al usuario mediante phishing o generar múltiples solicitudes de autenticación para conseguir que apruebe una solicitud maliciosa.

## SSO

**¿Qué es?**  
SSO (Single Sign-On) es un mecanismo que permite a un usuario autenticarse una vez y acceder posteriormente a múltiples aplicaciones o servicios sin volver a introducir sus credenciales.

**¿Dónde lo encuentro?**  
En organizaciones que centralizan el acceso a aplicaciones empresariales mediante un proveedor de identidad.

**¿Por qué me afecta?**  
Un compromiso de la cuenta o del proveedor de identidad puede proporcionar acceso a múltiples aplicaciones conectadas al sistema de SSO.

**¿Cómo se soluciona?**  
Protegiendo el proveedor de identidad con MFA resistente al phishing, mínimo privilegio, controles de sesión, monitoreo y políticas de acceso adecuadas.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede comprometer una cuenta utilizada para SSO y aprovechar las sesiones o permisos disponibles para acceder a múltiples servicios.

## Conditional Access

**¿Qué es?**  
Conditional Access es un mecanismo que aplica políticas de acceso basadas en condiciones como identidad, dispositivo, ubicación, riesgo o aplicación antes de permitir el acceso a un recurso.

**¿Dónde lo encuentro?**  
En plataformas de identidad empresariales y entornos cloud donde se utilizan políticas para controlar el acceso a aplicaciones y recursos.

**¿Por qué me afecta?**  
Una política mal configurada puede permitir accesos desde dispositivos, ubicaciones o situaciones que deberían considerarse riesgosas.

**¿Cómo se soluciona?**  
Definiendo políticas basadas en riesgo, aplicando MFA, restringiendo dispositivos no administrados y revisando periódicamente las excepciones y condiciones de acceso.

**¿Cómo lo usaría un atacante en mi contra?**  
Puede intentar acceder utilizando credenciales comprometidas desde una ubicación o dispositivo que cumpla las condiciones permitidas, o aprovechar excepciones mal configuradas.

## Zero Trust

**¿Qué es?**  
Zero Trust es un modelo de seguridad basado en el principio de no confiar automáticamente en usuarios, dispositivos o conexiones, incluso cuando se encuentran dentro de una red corporativa.

**¿Dónde lo encuentro?**  
En arquitecturas empresariales modernas que aplican controles de identidad, acceso, dispositivos, aplicaciones y redes de forma continua.

**¿Por qué me afecta?**  
Reduce el impacto de una cuenta o dispositivo comprometido al limitar el acceso únicamente a los recursos necesarios y verificar continuamente las condiciones de acceso.

**¿Cómo se soluciona?**  
Aplicando mínimo privilegio, autenticación fuerte, segmentación, verificación continua, controles de dispositivos y monitoreo de actividad.

**¿Cómo lo usaría un atacante en mi contra?**  
Intentará comprometer una identidad o dispositivo y utilizar los permisos disponibles para acceder a otros recursos, por lo que las debilidades en las políticas de Zero Trust pueden convertirse en rutas de movimiento lateral.
