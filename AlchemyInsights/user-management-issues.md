---
title: Problemas de administración de usuarios
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898167"
---
# <a name="user-management-issues"></a>Problemas de administración de usuarios

**¿Qué ocurre con los usuarios asignados actualmente a la aplicación si deshabilito la propiedad "Asignación de usuario necesaria" (establezco esta propiedad en No)?**

Deshabilitar la **Asignación de usuario necesaria** NO afecta a los usuarios asignados actualmente. Deshabilitar esta propiedad solo permitirá que todos los usuarios obtengan acceso a la aplicación. Todos los usuarios de la lista y los usuarios asignados a grupos en la aplicación seguirán siendo válidos.

- Para restringir la aplicación a un conjunto específico de usuarios, consulte [Restringir la aplicación de Azure AD a un conjunto de usuarios: Plataforma de identidad de Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Para asignar usuarios y grupos a aplicaciones empresariales en Azure Active Directory (Azure AD), ya sea desde el portal de Azure o mediante PowerShell, consulte [Administrar la asignación de usuarios de una aplicación en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Para delegar los permisos de administración y creación de aplicaciones, consulte [Delegar permisos de administrador para la administración de aplicaciones: Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Ocultar aplicaciones empresariales específicas para los usuarios** - Siga los siguientes pasos para ocultar todas las aplicaciones de Microsoft 365 desde el panel **Mis aplicaciones**. Las aplicaciones permanecerán visibles en el portal de Office 365.

 1. Inicie sesión en Azure portal como administrador global de su directorio. 
 2. Seleccione **Azure Active Directory**. 
 3. Seleccione **Usuarios**. 
 4. Seleccione **Configuración de usuario**. 
 5. En **Aplicaciones empresariales**, haga clic en **Administrar cómo los usuarios finales inician y ven sus aplicaciones**. 
 6. Para **Los usuarios solo pueden ver las aplicaciones de Office 365 en el portal de Office 365**, haga clic en **Sí**. 
 7. Haga clic en **Guardar**. 
 8. Para obtener más información, consulte [Ocultar una aplicación empresarial de la experiencia del usuario en Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Si ofrece una aplicación de Software como servicio (SaaS) para muchas organizaciones, puede configurarla para que acepte inicios de sesión desde cualquier espacio empresarial de Azure Active Directory (Azure AD). Esta configuración se denomina "hacer que su aplicación sea multiempresa". Los usuarios de cualquier espacio empresarial de Azure AD podrán iniciar sesión en la aplicación después de dar su consentimiento para usar su cuenta con ella. Para obtener más información, consulte [Crear aplicaciones que inicien sesión en los usuarios de Azure AD: Plataforma de identidad de Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **¿Cómo puede un usuario final tener acceso a la aplicación una vez que está asignado a ella?**

Cada aplicación de la hoja de la aplicación de Enterprise tiene un vínculo para que los usuarios finales puedan obtener acceso a ellas. Los usuarios también pueden acceder a la aplicación de un modo sencillo a través del portal **Mis aplicaciones**.

- **¿Quiere saber qué aplicaciones y tipos de aplicaciones están en uso por los usuarios?**

Puede descargar los informes de inicio de sesión de los últimos 30 días desde **portal.azure.com > Azure Active Directory> Inicios de sesión> descargar informes**.

- Obtenga información sobre cómo [Conceder permisos de administrador para el espacio empresarial en una aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) y [Configurar cómo los usuarios finales conceden permisos a las aplicaciones](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Comprender [cómo funciona el consentimiento de permisos](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) y [Administrar el consentimiento para aplicaciones](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


