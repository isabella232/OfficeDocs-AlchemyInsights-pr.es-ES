---
title: Eliminar permanentemente un sitio de SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771738"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="276aa-102">Eliminar permanentemente un sitio de SharePoint</span><span class="sxs-lookup"><span data-stu-id="276aa-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="276aa-103">Para volver a usar una dirección URL de un sitio eliminado (para volver a crear un sitio) o para eliminar permanentemente un sitio porque ya no está en uso, puede usar **Eliminar permanentemente** del nuevo Centro de administración de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="276aa-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="276aa-104">Vaya a la página [Sitios eliminados del nuevo Centro de administración de SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e inicie sesión con una cuenta que tenga permisos de administrador para su organización.</span><span class="sxs-lookup"><span data-stu-id="276aa-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="276aa-105">En la columna de la izquierda, seleccione un sitio.</span><span class="sxs-lookup"><span data-stu-id="276aa-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="276aa-106">Haga clic en **Eliminar permanentemente**</span><span class="sxs-lookup"><span data-stu-id="276aa-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="276aa-107">**Tenga en cuenta**: los sitios conectados a un grupo no se pueden eliminar permanentemente desde el nuevo Centro de administración de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="276aa-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="276aa-108">Se debe usar [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) en su lugar.</span><span class="sxs-lookup"><span data-stu-id="276aa-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="276aa-109">Para obtener más información, vea [Eliminar de forma permanente un sitio](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="276aa-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
