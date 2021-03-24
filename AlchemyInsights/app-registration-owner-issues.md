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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123197"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="a7b7f-102">Problemas del propietario del registro de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="a7b7f-102">App Registration Owner issues</span></span>

<span data-ttu-id="a7b7f-103">Estos son los métodos disponibles para agregar entidades de seguridad como propietarios para los registros de aplicaciones:</span><span class="sxs-lookup"><span data-stu-id="a7b7f-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="a7b7f-104">Uso del módulo de PowerShell de Azure AD:</span><span class="sxs-lookup"><span data-stu-id="a7b7f-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="a7b7f-105">Referencia: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="a7b7f-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="a7b7f-106">Uso de la CLI de Azure: `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="a7b7f-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="a7b7f-107">Referencia: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="a7b7f-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="a7b7f-108">Uso de MS Graph :</span><span class="sxs-lookup"><span data-stu-id="a7b7f-108">Using MS Graph -</span></span>

    <span data-ttu-id="a7b7f-109">Referencia: [Agregar propietario - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="a7b7f-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="a7b7f-110">Uso del Portal de Azure AD: vaya [a portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Select your application > Owners > Add Owners</span><span class="sxs-lookup"><span data-stu-id="a7b7f-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="a7b7f-111">**¿No puede ver la aplicación en la hoja Registros de aplicaciones aunque sea el propietario de esa aplicación?**</span><span class="sxs-lookup"><span data-stu-id="a7b7f-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="a7b7f-112">El propietario de una aplicación no es un rol administrativo.</span><span class="sxs-lookup"><span data-stu-id="a7b7f-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="a7b7f-113">Si la configuración [Restringir el acceso al portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) de administración de Azure AD está habilitada, solo el administrador podrá ver las aplicaciones en el portal de registro de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="a7b7f-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="a7b7f-114">Para que un propietario pueda ver las aplicaciones, deshabilite esta configuración (Establezca esta opción en NO) o asigne un rol de administrador al propietario solo para la aplicación específica.</span><span class="sxs-lookup"><span data-stu-id="a7b7f-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="a7b7f-115">Sin embargo, para ello, necesitará una licencia de Azure AD Premium P2 y habilitar [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span><span class="sxs-lookup"><span data-stu-id="a7b7f-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
