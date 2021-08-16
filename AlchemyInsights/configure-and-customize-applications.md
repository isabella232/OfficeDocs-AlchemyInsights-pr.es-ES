---
title: Configurar y personalizar aplicaciones
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045005"
---
# <a name="configure-and-customize-applications"></a>Configurar y personalizar aplicaciones

**Configurar aplicaciones**

1. Inicio rápido: configurar las propiedades de una aplicación en el inquilino de [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) muestra cómo configurar algunas de las propiedades de una aplicación.
2. Para ayudar a integrar sus aplicaciones con Azure Active Directory, hemos desarrollado una colección de [tutoriales](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) que le guían a través de la configuración.
3. [Cómo configurar una aplicación proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) de aplicación le ayuda a comprender cómo configurar una aplicación proxy de aplicación en Azure AD para exponer las aplicaciones locales a la nube.
4. [Descargar PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)y configurar la aplicación: siga las instrucciones de Configurar *PingAccess* para Azure AD para proteger las aplicaciones publicadas mediante proxy de aplicación Microsoft Azure AD en el sitio web Ping Identity y descargue la versión más reciente de PingAccess.

**Errores de aplicación mal configurada (AADSTS650056)**

1. Asegúrese de que tiene acceso a la aplicación desde la dirección de inicio de sesión proporcionada por el propietario de la aplicación. De lo contrario, inicie sesión en la aplicación a través de su proceso normal. En la mayoría de los casos, esto se resolverá automáticamente de forma natural. Si no lo hace, esta publicación puede ayudar a solucionar problemas y resolverlo.
2. **Si la organización es propietaria de la aplicación** (lo que significa que el registro de la aplicación está en la organización):
    - Como mínimo, se recomienda agregar el permiso delegado o de `User.Read` `openid` Microsoft **Graph.**
    - Asegúrese de que la aplicación y todos sus permisos están consintientes. Para comprobar esto, consulte  la columna Estado del registro de la aplicación en **Permisos de api**.
    - En algunos escenarios, la aplicación puede ser de terceros, pero puede estar registrada en su organización. Confirme si esta aplicación aparece en los registros de la aplicación (no Enterprise aplicaciones).
    - Si sigues consultando este mensaje de error. A continuación, es posible que deba crear la dirección URL de consentimiento descrita en **el paso 4**.
3. **Si su organización no es el propietario de la aplicación y la usa como una** aplicación de terceros:
    - Si es el administrador global/de la empresa, debería ver la pantalla de consentimiento. Asegúrese de marcar la casilla **"Consentimiento en nombre de su organización".**
    - Si no ve la pantalla de consentimiento, elimine la Enterprise y vuelva a intentarlo.
    - Si sigues consultando este mensaje de error. A continuación, es posible que deba crear la dirección URL de consentimiento descrita en **el paso 4**.
4. **Cree manualmente** la dirección URL de consentimiento que se usará: si la aplicación está diseñada para tener acceso a un recurso específico, es posible que no pueda usar los botones De consentimiento desde Azure Portal, deberá generar manualmente su propia dirección URL de consentimiento y usarla.
    - Deberá obtener el y `{App-Id}` el del propietario de la `{App-Uri-Id}` aplicación. `{Tenant-Id}` será el identificador de inquilino. Este será o `yourdomain.onmicrosoft.com` el id. de directorio.
    - Si la aplicación tiene acceso a sí misma para el recurso, `{App-Id}` el y será el `{App-Uri-Id}` mismo.
5. Para obtener más información, vea Problemas al iniciar sesión en aplicaciones configuradas de inicio de sesión [único basadas en SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizar aplicaciones**

- Agregar [personalización](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) de marca a la página de inicio de sesión de Azure Active Directory de la organización: use el logotipo de la organización y las esquemas de color personalizadas para proporcionar una apariencia coherente a las páginas de inicio de sesión de Azure Active Directory (Azure AD).
- [Agregar el nombre de dominio personalizado mediante el portal de Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) cada nuevo inquilino de Azure AD viene con un nombre de dominio inicial. No puede cambiar ni eliminar el nombre de dominio inicial, pero puede agregar los nombres de su organización. Agregar nombres de dominio personalizados le ayuda a crear nombres de usuario que estén familiarizados con los usuarios.
