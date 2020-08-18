---
title: Creación de un sitio de SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786582"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="4f130-102">Creación de un sitio de SharePoint</span><span class="sxs-lookup"><span data-stu-id="4f130-102">Create a SharePoint site</span></span>

<span data-ttu-id="4f130-103">Cree o administre sitios desde [sitios activos](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) en el centro de administración de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4f130-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="4f130-104">Para obtener más información, vea [administrar sitios en el nuevo centro de administración de SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4f130-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="4f130-105">Abrevia</span><span class="sxs-lookup"><span data-stu-id="4f130-105">Tips:</span></span>

- <span data-ttu-id="4f130-106">**No se puede** crear un sitio con la misma dirección URL de un sitio existente.</span><span class="sxs-lookup"><span data-stu-id="4f130-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="4f130-107">Si ha eliminado un sitio y desea volver a usar la dirección URL, es posible que el sitio eliminado siga existiendo en [sitios eliminados](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="4f130-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="4f130-108">El sitio tendrá que eliminarse de forma permanente para volver a usar la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="4f130-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="4f130-109">Para quitar por completo un sitio con PowerShell, consulte el ejemplo del cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="4f130-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="4f130-110">Es posible que algunos usuarios no puedan crear un sitio.</span><span class="sxs-lookup"><span data-stu-id="4f130-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="4f130-111">[Consulte administrar la creación de sitios en SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4f130-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="4f130-112">Es posible que el sitio aparezca bloqueado en la **creación** de más tiempo del esperado.</span><span class="sxs-lookup"><span data-stu-id="4f130-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="4f130-113">Si ha pasado más de 24 horas desde que vio por primera vez este problema, registre un vale de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="4f130-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4f130-114">En muchos casos, ya estamos trabajando en una solución.</span><span class="sxs-lookup"><span data-stu-id="4f130-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4f130-115">Por lo menos, danos 24 horas para completar una soluci? a.</span><span class="sxs-lookup"><span data-stu-id="4f130-115">Please give us at least 24 hours to complete a solution.</span></span>
