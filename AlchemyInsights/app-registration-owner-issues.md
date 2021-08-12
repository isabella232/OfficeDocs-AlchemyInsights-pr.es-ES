---
title: Problemas del propietario del registro de aplicaciones
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951150"
---
# <a name="app-registration-owner-issues"></a>Problemas del propietario del registro de aplicaciones

Estos son los métodos disponibles para agregar entidades de seguridad como propietarios para los registros de aplicaciones:

- Uso del módulo de PowerShell de Azure AD:

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referencia: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Uso de la CLI de Azure: `az ad app owner add`

    Referencia: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Uso de MS Graph -

    Referencia: [Agregar propietario: Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Uso del Portal de Azure AD: vaya [a portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Select your application > Owners > Add Owners

**¿No puede ver la aplicación en la hoja Registros de aplicaciones aunque sea el propietario de esa aplicación?**

El propietario de una aplicación no es un rol administrativo. Si la configuración [Restringir el acceso al portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) de administración de Azure AD está habilitada, solo el administrador podrá ver las aplicaciones en el portal de registro de aplicaciones. Para que un propietario pueda ver las aplicaciones, deshabilite esta configuración (Establezca esta opción en NO) o asigne un rol de administrador al propietario solo para la aplicación específica. Sin embargo, para ello, necesitará una licencia Azure AD Premium P2 y [habilitará Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
