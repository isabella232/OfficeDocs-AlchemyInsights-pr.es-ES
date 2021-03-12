---
title: Solucionar problemas de inicio de sesión único (SSO) basado en OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726943"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Solucionar problemas de inicio de sesión único (SSO) basado en OIDC

- Para obtener información sobre cómo agregar una aplicación basada en OIDC al inquilino de Azure, vea Inicio rápido: Configurar el inicio de sesión único (SSO) basado en OIDC para una aplicación en el inquilino de [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Para obtener más información acerca de las aplicaciones que usan el estándar OpenID Connect para implementar el inicio de sesión único, vea [Understand OIDC-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Para obtener información en caso de que elija escribir el código directamente enviando y controlando solicitudes HTTP o usando una biblioteca de código abierto de terceros, en lugar de usar una de nuestras bibliotecas de código abierto, vea [Protocolos OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)y OpenID Connect en la plataforma de identidades de Microsoft .

**Protocolos**

1. [Plataforma de identidades](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) de Microsoft y flujo de concesión implícito: la característica de definición de la concesión implícita es que los tokens (tokens de identificador o tokens de acceso) se devuelven directamente desde el extremo /authorize en lugar del extremo /token. Esto suele usarse como parte del flujo de código de autorización, en lo que se denomina **"flujo híbrido":** recuperar el token de identificador en la solicitud /authorize junto con un código de autorización . En este artículo se describe cómo programar directamente en el protocolo de la aplicación para solicitar tokens de Azure AD.
2. Flujo de código de autorización de la plataforma de identidades de Microsoft y [OAuth 2.0:](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) la concesión de código de autorización de OAuth 2.0 se puede usar en aplicaciones instaladas en un dispositivo para obtener acceso a recursos protegidos, como api web. Con la implementación de la plataforma de identidades de Microsoft de OAuth 2.0, puede agregar acceso de inicio de sesión y API a las aplicaciones móviles **y de escritorio.** En este artículo se describe cómo programar directamente en el protocolo de la aplicación con cualquier idioma.
3. Plataforma de identidades de Microsoft y protocolo [OpenID Connect:](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) cuando usa la implementación de OpenID Connect de la plataforma de identidades de Microsoft, puede agregar acceso a la API y el inicio de sesión a las aplicaciones. En este artículo se muestra cómo hacerlo independientemente del idioma y se describe cómo enviar y recibir mensajes HTTP sin usar bibliotecas de **código abierto de Microsoft.**
4. Plataforma de identidades de Microsoft y flujo de credenciales de cliente de [OAuth 2.0:](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) puede usar la concesión de credenciales de cliente de OAuth 2.0 especificada en RFC 6749, a veces denominada **OAuth** de dos patas, para obtener acceso a los recursos hospedados en web mediante la identidad de una aplicación. Este tipo de concesión se usa normalmente para las interacciones de servidor a servidor que deben ejecutarse en segundo plano, sin interacción inmediata con un usuario. Estos tipos de aplicaciones a menudo se conocen como **demonios o** cuentas **de servicio.** En este artículo se describe cómo programar directamente en el protocolo de la aplicación.
