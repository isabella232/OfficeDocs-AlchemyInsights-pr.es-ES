---
title: Problemas con tokens
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912037"
---
# <a name="issues-with-tokens"></a>Problemas con tokens

Para administrar problemas relacionados con tokens, puede dar los pasos siguientes:

1. Puede especificar la duración de un token de acceso, de SAML o de Id. emitido por la Plataforma de identidad de Microsoft. Establezca la vigencia de los tokens de todas las aplicaciones de su organización, de una aplicación de varios inquilinos (de varias organizaciones) o de una entidad de servicio de seguridad de la organización. Para más información, consulte [Vigencia de tokens configurable en la Plataforma de identidad de Microsoft (vista previa)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Los tokens de acceso permiten a los clientes llamar con seguridad API web protegidas y las API web los utilizan para realizar la autorización y autenticación. En conformidad con la especificación OAuth, los tokens de acceso son cadenas opacas sin formato establecido; algunos proveedores de identidad (IDP) utilizan GUID, otros emplean blobs cifrados. La Plataforma de identidad de Microsoft usa una variedad de formatos de token de acceso, en función de la configuración de la API que acepte el token. Para aprender cómo su API puede validar y usar las notificaciones dentro de un token de acceso, consulte [Token de acceso de la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. La Biblioteca de autenticación de Microsoft (MSAL) admite varios flujos de autenticación para usarlos en diferentes escenarios de aplicación. Para más información, consulte [Flujos de autenticación](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. La concesión del código de autorización OAuth 2.0 puede usarse en aplicaciones que estén instaladas en un dispositivo para obtener acceso a recursos protegidos, tales como API web. Si usa la implementación de OAuth 2.0 de la Plataforma de identidad de Microsoft, puede agregar inicio de sesión y acceso de API a sus aplicaciones de escritorio y de dispositivo móvil. Consulte el [Flujo del código de autorización de OAuth 2.0 y la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) para aprender a programar directamente contra el protocolo en su aplicación, en cualquier idioma.
5. OpenID Connect (OIDC) es un protocolo de autenticación creado en OAuth 2.0 que puede usar para que un usuario inicie sesión en una aplicación de manera segura. Al usar la implementación de OpenID Connect del punto de conexión de la Plataforma de identidad de Microsoft, puede agregar inicio de sesión y acceso de API a sus aplicaciones. El [Protocolo de OpenID Connect y la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) muestra cómo hacer esto sin importar el idioma y describe cómo enviar y recibir mensajes de HTTP sin usar ninguna biblioteca de fuente abierta de Microsoft.
    - El punto de conexión UserInfo forma parte del estándar OIDC, diseñado para devolver notificaciones sobre el usuario que ha realizado la autenticación. Para más información, consulte [Punto de conexión UserInfo de la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Este ejemplo de [llamada a una API web en una aplicación web mediante Azure AD y OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) muestra cómo crear una aplicación web de MVC que use Azure AD para iniciar sesión con el protocolo OpenID Connect y, después, realizar llamadas a una API web con la identidad del usuario que inició sesión mediante tokens obtenidos con OAuth 2.0. En este ejemplo, se usa el software intermedio de ASP .NET OWIN de OpenID Connect y ADAL .NET.
6. [Configurar una aplicación para exponer una API web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis): en esta guía de inicio rápido, puede registrar una API web con la Plataforma de identidad de Microsoft y exponerla a aplicaciones del cliente al agregar un ámbito de ejemplo. Al registrar su API web y exponerla mediante ámbitos, puede proporcionar acceso basado en permisos a sus recursos a usuarios autorizados y a aplicaciones cliente que acceden a su API.
7. En Azure Active Directory B2C (Azure AD B2C), el flujo de credenciales de contraseña del propietario del recurso (ROPC) es un flujo OAuth de autenticación estándar. En este flujo, una aplicación, también conocida como el usuario de confianza, intercambia credenciales válidos por tokens. Las credenciales incluyen una Id. de usuario y contraseña. Los tokens devueltos son un token de Id, de acceso y de actualización. Para más información, consulte [Establecer un flujo de credenciales de contraseña del propietario del recurso en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

