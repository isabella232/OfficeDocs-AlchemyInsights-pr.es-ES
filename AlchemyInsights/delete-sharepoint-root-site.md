---
title: Eliminar el sitio de raíz de SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815488"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="ee815-102">Eliminar el sitio de raíz de SharePoint</span><span class="sxs-lookup"><span data-stu-id="ee815-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="ee815-103">**No se admite** la eliminación del sitio de raíz de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ee815-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="ee815-104">Si el sitio de raíz ya se ha eliminado, los usuarios recibirán un error 404 Archivo no encontrado si intentan acceder al sitio en cuestión.</span><span class="sxs-lookup"><span data-stu-id="ee815-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="ee815-105">Para resolver el problema, restaure el sitio desde el Centro de administración de SharePoint. Para ello, vaya a la página [Sitios eliminados](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true), seleccione el sitio de raíz y haga clic en Restaurar.</span><span class="sxs-lookup"><span data-stu-id="ee815-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="ee815-106">En lugar de eliminar el sitio de raíz, utilice [reemplazar sitio](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) desde el nuevo Centro de administración de SharePoint una vez que el sitio de raíz haya sido restaurado.</span><span class="sxs-lookup"><span data-stu-id="ee815-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="ee815-107">Para obtener más información sobre los requisitos, consulte [Modernizar el sitio raíz](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="ee815-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>