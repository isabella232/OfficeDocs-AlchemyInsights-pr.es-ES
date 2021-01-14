---
title: Problemas con la integración de SSO de conexión directa con mis aplicaciones locales
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848781"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemas con la integración de SSO de conexión directa con mis aplicaciones locales

Para solucionar problemas relacionados con la integración de SSO de conexión directa con aplicaciones locales, haga lo siguiente:

**Pasos recomendados**

1. Para configurar una **aplicación local** para el inicio de sesión único a través del **Proxy** de aplicación, consulte Almacén de contraseñas para el inicio de sesión único con proxy [de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Solución de problemas de Proxy** de aplicación: se recomienda empezar con la revisión del flujo de solución de problemas, depurar problemas del conector de [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)de aplicación para determinar si los conectores de proxy de aplicación están configurados correctamente. Si sigue teniendo problemas para conectarse a la aplicación, siga los pasos de solución de problemas de depurar problemas de [la aplicación proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Puede identificar [problemas de CORS mediante](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) las siguientes herramientas de depuración del explorador:
    1. Inicie el explorador y vaya a la aplicación web.
    1. Presione **F12 para** abrir la consola de depuración.
    1. Intente reproducir la transacción y revise el mensaje de la consola. Una infracción de CORS produce un error de consola sobre el origen.
    1. Algunos problemas de CORS no se pueden resolver, como cuando la aplicación redirige a login.microsoftonline.com para autenticarse y el token de acceso expira. A continuación, se produce un error en la llamada cors. Una solución alternativa para este escenario es ampliar la duración del token de acceso para evitar que expire durante la sesión de un usuario. Para obtener más información acerca de cómo hacerlo, vea [Vigencia de tokens configurables en la plataforma de identidad de Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Documentos recomendados**

- [Cómo configurar el inicio de sesión único en una aplicación proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Inicio de sesión único SAML para aplicaciones locales con Proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Comprender y resolver problemas de CORS del proxy de aplicación de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Solucionar problemas de las configuraciones de delegación limitada de Kerberos para proxy de aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)