---
title: Eliminar o restaurar aplicaciones
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013986"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="adb71-102">Eliminar o restaurar aplicaciones</span><span class="sxs-lookup"><span data-stu-id="adb71-102">Delete or restore applications</span></span>

<span data-ttu-id="adb71-103">**Para eliminar una aplicación del inquilino de Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="adb71-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="adb71-104">En el **portal de Azure AD,** seleccione **Aplicaciones de empresa.**</span><span class="sxs-lookup"><span data-stu-id="adb71-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="adb71-105">A continuación, busque y seleccione la aplicación que desea eliminar.</span><span class="sxs-lookup"><span data-stu-id="adb71-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="adb71-106">En la **sección** Administrar del panel izquierdo, seleccione **Propiedades**.</span><span class="sxs-lookup"><span data-stu-id="adb71-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="adb71-107">Seleccione **Eliminar** y, a continuación, seleccione **Sí** para confirmar que desea eliminar la aplicación del inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="adb71-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="adb71-108">Para obtener más información sobre cómo eliminar una aplicación, vea Inicio rápido: Eliminar una aplicación de su inquilino de [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="adb71-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="adb71-109">En PowerShell, el cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) quita las configuraciones de Proxy de aplicación de una aplicación específica en Azure Active Directory y puede eliminar la aplicación por completo si se especifica.</span><span class="sxs-lookup"><span data-stu-id="adb71-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="adb71-110">Puede restaurar **una aplicación eliminada con** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="adb71-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="adb71-111">Una vez identificada la aplicación que desea restaurar, puede restaurarla con [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="adb71-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
