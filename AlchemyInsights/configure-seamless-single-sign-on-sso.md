---
title: Configurar el inicio de sesión único sin problemas (SSO)
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/15/2021
ms.locfileid: "50819592"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurar el inicio de sesión único sin problemas (SSO)

**Configurar aplicaciones**

1. Debe obtener los valores del proveedor de aplicaciones. Puede escribir manualmente los valores o cargar un archivo de metadatos para extraer el valor de los campos.
2. Muchas aplicaciones ya se han configurado previamente para funcionar con Azure AD. Estas aplicaciones se enumeran en la galería de aplicaciones que puedes examinar cuando agregas una aplicación a tu inquilino de Azure AD. La [serie de inicio rápido](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) le guiará por el proceso.
3. Para crear una aplicación que no es de galería, puede hacer clic en **+ Crear su** propio botón Aplicación y dar un nombre a la aplicación.
    - De forma predeterminada, seleccionará **Integrar cualquier otra** aplicación que no encuentre en la galería, que es la opción correcta para aplicaciones que no son de galería.
    - Una vez que presione **Crear** después de colocar el nombre de la aplicación, creará una nueva aplicación de empresa que no sea de galería.
    - A continuación, puede navegar hasta **Inicio** de sesión único en **Administrar** de esa aplicación y podrá ver distintas técnicas para implementarla en su entorno.

**Configurar SSO de conexión directa para una aplicación específica**

Para las aplicaciones de la galería, encontrará instrucciones detalladas, paso a paso. Para obtener acceso a los pasos, puede examinar una lista de todos los tutoriales de configuración de aplicaciones en los tutoriales de configuración de aplicaciones [SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Configurar SSO basado en SAML**

1. Inicio rápido: Configurar el inicio de sesión único (SSO) basado en SAML para una aplicación en el inquilino de [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Para obtener más información sobre la opción basada en SAML para el inicio de sesión único, vea [Understand SAML-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Para obtener información sobre las solicitudes y respuestas de autenticación SAML 2.0 que Azure Active Directory (Azure AD) admite para single Sign-On (SSO), consulte [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Para obtener información sobre cómo crear y configurar un inicio de sesión único (SSO) basado en SAML para la aplicación en Azure Active Directory (Azure AD) mediante la API de Microsoft Graph, vea [Configure SAML-based single sign-on for your application using the Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Para obtener información sobre cómo Azure AD usa el protocolo SAML, consulte [How the Microsoft identity platform uses the SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Configurar tokens y notificaciones**

1. [Cómo personalizar las notificaciones emitidas en el token SAML para aplicaciones empresariales](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Para obtener información sobre cómo configurar notificaciones con PowerShell, vea [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Para obtener información sobre cómo configurar notificaciones opcionales, consulta [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Para obtener información sobre cómo usar atributos de extensión de esquema de directorio para enviar datos de usuario a aplicaciones en notificaciones de token, vea [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Para obtener información sobre cómo configurar las duraciones de token, consulte [Configurable token lifetimes in the Microsoft identity platform (preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Configurar directivas de vigencia de token (versión preliminar):](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) en este artículo, se describe un escenario de directiva común que puede ayudarle a imponer nuevas reglas para la duración del token. En el ejemplo, aprenderás a crear una directiva que requiera que los usuarios se autentiquen con más frecuencia en la aplicación web.

**Solucionar problemas de configuración de SSO**

- Para obtener preguntas más frecuentes acerca de Azure Active Directory Seamless Single Sign-On (SSO de conexión directa), consulte Inicio de sesión único sin problemas de [Azure Active Directory: preguntas más frecuentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Para solucionar problemas relacionados con problemas comunes relacionados con Azure Active Directory (Azure AD) Seamless Single Sign-On (SSO de conexión directa), consulte [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
