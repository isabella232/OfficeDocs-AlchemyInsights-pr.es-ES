---
title: Errores de aplicación
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976937"
---
# <a name="application-errors"></a>Errores de aplicación

¿Está buscando información sobre los códigos de error de **AADSTS** que se devuelven desde el servicio de token de seguridad (STS) de Azure Active Directory (Azure AD)? Lea [los códigos de error de autenticación](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) y autorización de Azure AD para encontrar descripciones de errores de AADSTS, correcciones y algunas soluciones alternativas sugeridas.

Los errores de autorización pueden ser el resultado de varios problemas diferentes, la mayoría de los cuales generan un error 401 o 403. Por ejemplo, lo siguiente puede dar lugar a errores de autenticación:

- [Flujos de adquisición de token de acceso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorrectos 
- [Ámbitos de permiso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurado 
- Ausencia de [consentimiento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Para resolver errores comunes de autorización, pruebe los pasos que se indican a continuación que coincidan más estrechamente con el error que está recibiendo. Se pueden aplicar más de uno.

**Error 401 No autorizado: ¿es válido el token?**

Asegúrese de que la aplicación presenta un token de acceso válido a Microsoft Graph como parte de la solicitud. Este error suele indicar que es posible que falte el token de acceso en el encabezado de solicitud de autenticación HTTP o que el token no sea válido o haya expirado. Le recomendamos encarecidamente que use la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) para la adquisición de tokens de acceso. Además, este error puede producirse si intenta usar un token de acceso delegado concedido a una cuenta personal de Microsoft para tener acceso a una API que solo admite cuentas de trabajo o educativas (cuentas organizativas).

**Error 403 Prohibido: ¿ha elegido el conjunto adecuado de permisos?**

Compruebe que ha solicitado el conjunto correcto de permisos en función de las API de Microsoft Graph a las que llama la aplicación. Los permisos con privilegios mínimos recomendados se proporcionan en todos los temas del método de referencia de la API de Microsoft Graph. Además, un usuario o un administrador deben conceder estos permisos a la aplicación. La concesión de permisos suele hacerse con una página de consentimiento o concediendo permisos mediante la hoja de registro de aplicaciones del portal de Azure. En la hoja **Configuración** de la aplicación, haga clic en **Permisos necesarios** y haga clic en **Conceder permisos**.

- [Permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Descripción de permisos y consentimiento de Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Error 403 Prohibido: ¿ha adquirido su aplicación un token para coincidir con los permisos seleccionados?**

Asegúrese de que el tipo de permisos solicitado o concedido coincida con el tipo de token de acceso que la aplicación adquiere. Es posible que solicite y conceda permisos de aplicación, pero que use tokens de flujo de código interactivo delegados en lugar de tokens de flujo de credenciales de cliente, o bien que solicite y conceda permisos delegados, pero que utilice tokens de flujo de credenciales de cliente en lugar de los tokens de flujo de código delegado.

- [Obtener acceso en nombre de usuarios y permisos delegados](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0: Flujo de código de autenticación de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obtener acceso sin usuario (servicio de demonio) y permisos de aplicación](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0: Flujo de credenciales de cliente de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Error 403 Prohibido:: restableciendo contraseña**

Actualmente, no hay permisos de servicio a servicio de demonio de permiso de aplicación que permitan restablecer las contraseñas de usuario. Las API solo se admiten con el código delegado interactivo en los flujos con una sesión de administrador iniciada.

- [Permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**Error 403 Prohibido: ¿tiene acceso el usuario y está autorizado?**

Para flujos de código delegados, Microsoft Graph evalúa si la solicitud se permite en función de los permisos concedidos a la aplicación y los permisos que tiene el usuario que ha iniciado sesión. Por lo general, este error indica que el usuario no tiene privilegios suficientes para realizar la solicitud o el usuario no tiene licencia para tener acceso a los datos. Solo los usuarios con los permisos o licencias necesarios pueden realizar la solicitud correctamente.

**Error 403 Prohibido: ¿seleccionó la API de recurso adecuada?**

Los servicios de API como Microsoft Graph comprueban que la notificación de aud (audiencia) en el token de acceso recibido coincide con el valor que espera para sí mismo y, si no es así, produce un error 403 Prohibido. Un error común que resulta en este error es intentar usar un token adquirido para las API de Azure AD Graph, las API de Outlook o las API de SharePoint/OneDrive para llamar a Microsoft Graph (o viceversa). Asegúrese de que el recurso (o ámbito) para el que la aplicación está adquiriendo un token coincida con la API a la que llama la aplicación.

**400 Solicitud incorrecta o 403 Prohibido: ¿cumple el usuario las directivas de acceso condicional (CA) de su organización?**

En función de las directivas de ca de una organización, un usuario que obtiene acceso a los recursos de Microsoft Graph a través de la aplicación puede ser objeto de un desafío por información adicional que no está presente en el token de acceso que adquirió originalmente la aplicación. En este caso, la aplicación recibe un error 400 con *interaction_required* durante la adquisición del token de acceso o un error 403 con *insufficient_claims* cuando se llama a Microsoft Graph. En ambos casos, la respuesta del error contiene información adicional que puede mostrarse al punto de conexión de autorización para pedir al usuario información adicional (por ejemplo, autenticación multifactor o inscripción de dispositivo).

- [Controlar los desafíos de acceso condicional mediante MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Guía para desarrolladores para acceso condicional de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
