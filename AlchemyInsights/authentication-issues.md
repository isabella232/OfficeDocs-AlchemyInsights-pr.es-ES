---
title: Problemas de autenticación
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976866"
---
# <a name="authentication-issues"></a>Problemas de autenticación

**¿Busca información sobre los códigos de error que devuelve el servicio de token de seguridad (STS) de Azure Active Directory (Azure AD)?** Consulte [códigos de error de autorización y Autenticación de Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) encontrar descripciones de errores, correcciones y algunas soluciones alternativas sugeridas para AADSTS.

Los errores de autorización pueden ser el resultado de varios problemas diferentes, la mayoría de los cuales generan un error 401 o 403. Por ejemplo, los siguientes problemas pueden causar errores de autorización:

- [Flujos de adquisición de token de acceso](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorrectos 
- [Ámbitos de permiso](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) mal configurado 
- Ausencia de [consentimiento](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Para resolver errores comunes de autorización, pruebe los pasos que se indican a continuación que coincidan mejor con el error que está obteniendo. Es posible que se aplique más de un paso para un error que está obteniendo.

**Error 401 No autorizado: ¿es válido el token?**

Asegúrese de que la aplicación presenta un token de acceso válido a Microsoft Graph como parte de la solicitud. Este error suele indicar que es posible que falte el token de acceso en el encabezado de solicitud de autenticación HTTP o que el token no sea válido o haya expirado. Le recomendamos encarecidamente que use la biblioteca de autenticación de Microsoft (MSAL) para la adquisición de tokens de acceso. Además, este error puede producirse si intenta usar un token de acceso delegado concedido a una cuenta de Microsoft personal para tener acceso a una API que solo admite cuentas profesionales o educativas (cuentas de organización).

**Error 403 Prohibido: ¿ha elegido el conjunto adecuado de permisos?**

Asegúrese de que ha solicitado el conjunto de permisos correcto en función de las API de Microsoft Graph a las que llama la aplicación. Los permisos con menos privilegios recomendados se proporcionan en todos los temas sobre el método de referencia de la API de Microsoft Graph. Además, un usuario o un administrador deben conceder estos permisos a la aplicación. La concesión de permisos suele hacerse con una página de consentimiento o el uso de la hoja de registro de aplicaciones de Azure Portal. En la hoja **Configuración** de la aplicación, haga clic en **Permisos necesarios** y haga clic en **Conceder permisos**. Para más información, vea:

- [Permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Descripción de permisos y consentimiento de Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Error 403 Prohibido: ¿ha adquirido su aplicación un token para coincidir con los permisos seleccionados?**

Asegúrese de que los tipos de permisos solicitados o concedidos coincidan con el tipo de token de acceso que la aplicación adquiere. Es posible que solicite y conceda permisos de aplicación, pero que use tokens de flujo de código interactivo delegados en lugar de tokens de flujo de credenciales de cliente, o bien que solicite y conceda permisos delegados, pero que utilice tokens de flujo de credenciales de cliente en lugar de los tokens de flujo de código delegado.

Para más información relacionada con la adquisición de tokens, consulte:

- [Obtener acceso en nombre de usuarios y permisos delegados](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0: Flujo de código de autenticación de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obtener acceso sin usuario (servicio de demonio) y permisos de aplicación](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0: Flujo de credenciales de cliente de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Error 403 Prohibido:: restableciendo contraseña**

Actualmente, no hay permisos de servicio a servicio de demonio de permiso de aplicación que permitan restablecer las contraseñas de usuario. Las API solo se admiten con el código delegado interactivo en los flujos con una sesión de administrador iniciada. Para más información, vea [Permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**Error 403 Prohibido: ¿tiene acceso el usuario y está autorizado?**

En el caso de los flujos de código delegado, Microsoft Graph evalúa si se ha permitido la solicitud en función de los permisos concedidos a la aplicación y los permisos que tiene el usuario que ha iniciado sesión. Por lo general, este error indica que el usuario no tiene privilegios suficientes para realizar la solicitud **o** el usuario no tiene licencia para tener acceso a los datos. Solo los usuarios con los permisos o licencias necesarios pueden realizar la solicitud correctamente.

**Error 403 Prohibido: ¿seleccionó la API de recurso adecuada?**

Los servicios de API como Microsoft Graph comprueban que la notificación *aud* (audiencia) en el token de acceso recibido coincida con el valor que espera para sí mismo y, si no es así, se produce un error 403 Prohibido. Un fallo común que provoca este error es cuando se intenta usar un token adquirido para las API de Azure AD Graph, las API de Outlook o las API de SharePoint o OneDrive para llamar a Microsoft Graph (o viceversa). Asegúrese de que el recurso (o ámbito) para el que la aplicación está adquiriendo un token coincida con la API a la que llama la aplicación.

**400 Solicitud incorrecta o 403 Prohibido: ¿cumple el usuario las directivas de acceso condicional (CA) de su organización?**

En función de las directivas de acceso condicional (CA) de una organización, un usuario que tenga acceso a los recursos de Microsoft Graph a través de la aplicación podría tener dificultades para obtener información adicional que no se encuentre en el token de acceso que ha adquirido originalmente la aplicación. En este caso, la aplicación recibe un error **400 con *interaction_required*** durante la adquisición del token de acceso o un error **403 con *insufficient_claims*** cuando se llama a Microsoft Graph. En ambos casos, la respuesta del error contiene información adicional que puede mostrarse al punto de conexión autorizado para pedir al usuario información adicional (por ejemplo, autenticación multifactor o inscripción de dispositivo).

Para más información relacionada con el acceso condicional, vea:

- [Manejar solicitudes de acceso condicional con MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Guía para desarrolladores para acceso condicional de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Fin de soporte para la Biblioteca de autenticación de Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)_* _

- A partir del 30 de junio de 2020, ya no agregaremos nuevas características a la Biblioteca de autenticación de Active Directory (ADAL) y a la API de Azure AD Graph (AAD Graph). Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.
- A partir del 30 de junio de 2022, finalizaremos el soporte para ADAL y Azure AD Graph y dejaremos de ofrecer soporte técnico o actualizaciones de seguridad.
    - Las aplicaciones que usen ADAL en versiones existentes del SO seguirán funcionando después de este momento, pero no recibirán actualizaciones de soporte técnico ni de seguridad.
    - Es posible que, después de este momento, las aplicaciones que usan AAD Graph ya no reciban respuestas del punto de conexión de AAD Graph.

_ *Migración de ADAL**

Se recomienda actualizar a la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tiene las últimas características y actualizaciones de seguridad. Esta recomendación se debe a que Microsoft migrará sus aplicaciones a MSAL antes de la fecha límite del fin de soporte técnico. El objetivo de la migración de aplicaciones de Microsoft a MSAL es asegurar que las aplicaciones se beneficien de las mejoras en características y seguridad continuas de MSAL.

- [Leer las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Obtener información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Si necesita ayuda para comprender cuáles de sus aplicaciones usan ADAL, le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier proveedor de software independiente (ISV) o proveedor de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de AAD Graph**

Para las aplicaciones que usan AAD Graph, siga nuestras instrucciones para [migrar aplicaciones de Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Nuestra lista de comprobación para la migración proporciona un punto de inicio](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier ISV o proveedor de aplicaciones que corresponda. El soporte técnico de Microsoft también puede proporcionarle la información de todo el uso de AAD Graph en su espacio empresarial.

 










