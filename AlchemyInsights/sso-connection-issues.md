---
title: Problemas de conexión sso
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918148"
---
# <a name="sso-connection-issues"></a>Problemas de conexión sso

1. Siga la guía [Inicio rápido: configurar las propiedades de una aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) para configurar la aplicación.
2. Según la aplicación y la [opción de inicio de sesión único](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que elija, siga las instrucciones adecuadas a continuación:
    - Para configurar una **aplicación local** para el inicio de sesión único basado en **SAML,** vea inicio de sesión único saml para aplicaciones locales [con proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Para configurar una **aplicación en la nube** para **el** inicio de sesión único basado en contraseña, vea Configurar el inicio de sesión único [de contraseña.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Para configurar una **aplicación local** para el inicio de sesión único a través del **Proxy** de aplicación, consulte Almacén de contraseñas para el inicio de sesión único con proxy [de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Solución de problemas de Proxy** de aplicación: se recomienda empezar con la revisión del flujo de solución de problemas, depurar problemas del conector de [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)de aplicación para determinar si los conectores de proxy de aplicación están configurados correctamente. Si todavía tiene problemas para conectarse a la aplicación, siga el flujo de solución de problemas en depurar problemas de [la aplicación proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Puede identificar [problemas de CORS con](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) las herramientas de depuración del explorador:
    - Inicie el explorador y busque la aplicación web.
    - Presione **F12** para abrir la consola de depuración.
    - Intente reproducir la transacción y revise el mensaje de la consola. Una infracción de CORS produce un error de consola sobre el origen.
    - Algunos problemas de CORS no se pueden resolver, como cuando la aplicación redirige a login.microsoft.com para autenticarse y el token de acceso expira. A continuación, se produce un error en la llamada cors. Una solución para este escenario es extender la duración del token de acceso para evitar que expire durante la sesión de un usuario. Para más información sobre cómo hacer esto, vea [Vigencia de tokens configurable en la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Solución de problemas del inicio de sesión único basado en **SAML:** le recomendamos que consulte Problemas al iniciar sesión en aplicaciones configuradas de inicio de sesión único basado en [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar las soluciones a los problemas que es más probable que encuentre.
5. **Solución de problemas del** inicio de sesión único basado en contraseña: recomendamos comprobar el inicio de sesión único basado en contraseña en [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar las soluciones a los problemas que son más probables que se encuentren.
6. Para ver los problemas de conexión al usar una VPN, consulte Cómo usar el inicio de sesión único [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)a través de VPN y Wi-Fi vpn.
