---
title: Solucionar problemas de inicio de sesión único (SSO) basado en contraseña
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
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709504"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Solucionar problemas de inicio de sesión único (SSO) basado en contraseña

Para obtener información sobre los conceptos básicos del SSO basado en contraseña, consulte Autenticación basada en [contraseñas con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurar SSO basado en contraseñas**

1. [Configurar el inicio de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) sesión único basado en contraseña: en este artículo se explica más detalladamente la opción sso basada en contraseña. Si la aplicación que está agregando requiere una configuración personalizada y necesita usar SSO basado en contraseña, este artículo es para usted.
2. [Configurar el inicio de sesión único](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) basado en contraseña para aplicaciones de inicio de sesión automático: el proxy de aplicación admite varios modos de inicio de sesión único. El inicio de sesión basado en contraseña está pensado para aplicaciones que usan una combinación de nombre de usuario y contraseña para la autenticación. Al configurar el inicio de sesión basado en contraseña para la aplicación, los usuarios deben iniciar sesión en la aplicación local una vez. Después, Azure Active Directory almacena la información de inicio de sesión y la proporciona automáticamente a la aplicación cuando los usuarios tienen acceso a ella de forma remota.
    - Ya deberías haber publicado y probado la aplicación con proxy de aplicación. Si no es así, siga los pasos descritos en Publicar aplicaciones con el proxy de aplicación de [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) y, a continuación, continúe con la configuración de SSO basado en contraseña para aplicaciones pre-instaladas.

Para solucionar problemas de SSO basado en contraseña, consulte Solucionar problemas de inicio de sesión único basado en [contraseña en Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
