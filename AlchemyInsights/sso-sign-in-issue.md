---
title: Problemas de inicio de sesión de usuario de SSO sin problemas
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919210"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problemas de inicio de sesión de usuario de SSO sin problemas

Una vez autenticado el usuario, el explorador almacenará en caché las credenciales del usuario para que, en el mismo explorador, la aplicación inicie sesión automáticamente con la misma cuenta. Esto puede dificultar que otro usuario o un único usuario inicie sesión en varias cuentas en un dispositivo. Para resolver esto: 1. Intente iniciar sesión en otro explorador. 2. Borre la memoria caché o las cookies del explorador e intente iniciar sesión de nuevo.

Si sigue experimentando problemas de inicio de sesión, se recomienda lo siguiente para diagnosticar y automatizar los pasos de resolución:

1. Instale la [extensión del](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) explorador seguro de Mis aplicaciones para ayudar a Azure Active Directory (Azure AD) a proporcionar un mejor diagnóstico y soluciones al usar la experiencia de prueba en Azure Portal.
2. Reproduzca el error con la experiencia de prueba en la página de configuración de la aplicación en Azure Portal. Para obtener más información, consulte Depurar aplicaciones de [inicio de sesión único basadas en SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Si usa la experiencia de prueba en Azure Portal con la Extensión de explorador seguro de Mis aplicaciones, puede omitir **el paso 4.**
4. Para abrir la página de configuración de inicio de sesión único basado en SAML:
    - Abra [Azure Portal e](https://portal.azure.com/) inicie sesión como administrador **global** o **coadmin.**
    - Abra la **Extensión de Azure Active Directory** seleccionando **Todos** los servicios en la parte superior del menú de navegación principal del lado izquierdo.
    - Escriba "Azure Active Directory" en el cuadro de búsqueda de filtros y seleccione el **elemento de Azure Active Directory.**
    - Seleccione **Aplicaciones de empresa en** el menú de navegación izquierdo de Azure Active Directory.
    - Seleccione **Todas las aplicaciones** para ver una lista de todas las aplicaciones. Si no ve la aplicación que desea que se muestre aquí,  use el **control** Filtro en la parte superior de la lista Todas las aplicaciones y establezca la opción Mostrar en Todas **las aplicaciones.** 
    - Seleccione la aplicación que desea configurar para el inicio de sesión único.
    - Después de cargar la aplicación, seleccione **Inicio de sesión único** en el menú de navegación izquierdo de la aplicación.
    - Seleccione **SSO basado en SAML.**
5. En función del error, para obtener más información sobre los pasos recomendados a seguir, vea Problemas al iniciar sesión en aplicaciones configuradas de inicio de sesión [único basado en SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Para solucionar otros problemas de inicio de sesión de usuario, consulte las siguientes instrucciones:
    - [Protocolo SAML Sign-On único](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Procedimiento para solucionar errores de inicio de sesión con informes de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Mensaje de consentimiento inesperado](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Error de consentimiento del usuario](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemas al iniciar sesión desde Mis aplicaciones](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Error en la página de inicio de sesión de la aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problema al iniciar sesión en una aplicación de Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
