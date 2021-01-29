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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2021
ms.locfileid: "50043990"
---
# <a name="configure-and-customize-applications"></a>Configurar y personalizar aplicaciones

**Configurar aplicaciones**

1. Inicio rápido: configurar las propiedades de una aplicación en el inquilino de [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) muestra cómo configurar algunas de las propiedades de una aplicación.
2. Para ayudar a integrar las aplicaciones con Azure Active Directory, hemos desarrollado una colección de [tutoriales](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) que le guían a través de la configuración.
3. [Cómo configurar una aplicación proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) de aplicación le ayuda a comprender cómo configurar una aplicación de proxy de aplicación en Azure AD para exponer las aplicaciones locales a la nube.
4. [Descargue PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)y configure la aplicación: siga las instrucciones de Configurar *PingAccess* para Azure AD para proteger las aplicaciones publicadas con el Proxy de aplicación de Microsoft Azure AD en el sitio web de Ping Identity y descargue la versión más reciente de PingAccess.

**Errores de aplicación mal configurada (AADSTS650056)**

1. Asegúrese de que tiene acceso a la aplicación desde la dirección de inicio de sesión proporcionada por el propietario de la aplicación. De lo contrario, inicie sesión en la aplicación a través de su proceso normal. En la mayoría de los casos, esto se resolverá automáticamente de forma natural. Si no lo hace, esta publicación puede ayudar a solucionar problemas y resolverlo.
2. **Si la organización es propietaria de la aplicación** (lo que significa que el registro de la aplicación está en la organización):
    - Como mínimo, se recomienda agregar el permiso delegado o `User.Read` `openid` de Microsoft **Graph.**
    - Asegúrese de que se da su consentimiento a la aplicación y a todos sus permisos. Para comprobarlo, consulte la columna **Estado** del registro de la aplicación en **Permisos de API.**
    - En algunos escenarios, la aplicación puede ser de terceros, pero puede estar registrada en la organización. Confirma si esta aplicación aparece en los registros de la aplicación (no en las aplicaciones de empresa).
    - Si sigues teniendo este mensaje de error. A continuación, es posible que tenga que crear la dirección URL de consentimiento descrita en **el paso 4.**
3. **Si su organización no es el propietario de la aplicación y la usa** como aplicación de terceros:
    - Si es el administrador global o de la compañía, debería ver la pantalla de consentimiento. Asegúrese de marcar la casilla **"Consentimiento en nombre de su organización"**.
    - Si no ve la pantalla de consentimiento, elimine la aplicación Enterprise e inténtelo de nuevo.
    - Si sigues teniendo este mensaje de error. A continuación, es posible que tenga que crear la dirección URL de consentimiento descrita en **el paso 4.**
4. **Cree** manualmente la dirección URL de consentimiento que se usará: si la aplicación está diseñada para tener acceso a un recurso específico, es posible que no pueda usar los botones de consentimiento desde Azure Portal, deberá generar manualmente su propia dirección URL de consentimiento y usarla.
    - Deberá obtener el propietario y `{App-Id}` el del propietario de la `{App-Uri-Id}` aplicación. `{Tenant-Id}` será su identificador de inquilino. Este será o `yourdomain.onmicrosoft.com` el id. de directorio.
    - Si la aplicación tiene acceso a sí misma para el recurso, `{App-Id}` el y será el `{App-Uri-Id}` mismo.
5. Para obtener más información, consulta Problemas al iniciar sesión en aplicaciones configuradas de [inicio de sesión único basado en SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizar aplicaciones**

- Agregue personalización de marca a la página de inicio de sesión de [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) de su organización: use el logotipo de su organización y las esquemas de colores personalizadas para proporcionar una apariencia coherente a las páginas de inicio de sesión de Azure Active Directory (Azure AD).
- [Agregue el nombre de dominio personalizado mediante el portal de Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) cada nuevo inquilino de Azure AD viene con un nombre de dominio inicial. No puede cambiar ni eliminar el nombre de dominio inicial, pero puede agregar los nombres de su organización. Agregar nombres de dominio personalizados le ayuda a crear nombres de usuario que sean familiares para los usuarios.
