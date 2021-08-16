---
title: Problemas con la integración de SSO sin problemas con mis aplicaciones locales
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028309"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemas con la integración de SSO sin problemas con mis aplicaciones locales

Para solucionar problemas relacionados con la integración de SSO sin problemas con aplicaciones locales, haga lo siguiente:

**Pasos recomendados**

1. Para configurar una **aplicación local para** el inicio de sesión único a través del **proxy** de aplicación, vea [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Solución de problemas de proxy** de aplicación: se recomienda empezar con la revisión del flujo de solución de problemas, depurar problemas del conector de [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)de aplicación , para determinar si los conectores de proxy de aplicación están configurados correctamente. Si sigue teniendo problemas para conectarse a la aplicación, siga los pasos de solución de problemas de [Depurar problemas de conectores proxy de aplicaciones](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Puede identificar [problemas cors mediante](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) las siguientes herramientas de depuración del explorador:
    1. Inicie el explorador y busque la aplicación web.
    1. Presione **F12** para abrir la consola de depuración.
    1. Intente reproducir la transacción y revise el mensaje de la consola. Una infracción de CORS produce un error de consola sobre el origen.
    1. Algunos problemas de CORS no se pueden resolver, como cuando la aplicación redirige a login.microsoftonline.com para autenticarse y el token de acceso expira. A continuación, se produce un error en la llamada CORS. Una solución para este escenario es extender la duración del token de acceso para evitar que expire durante la sesión de un usuario. Para más información sobre cómo hacer esto, vea [Vigencia de tokens configurable en la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documentos recomendados**

- [Cómo configurar el inicio de sesión único en una aplicación proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Inicio de sesión único SAML para aplicaciones locales con proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Comprender y resolver problemas Azure Active Directory CORS de proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Solución de problemas con las configuraciones de delegación restringidas de Kerberos para Proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)