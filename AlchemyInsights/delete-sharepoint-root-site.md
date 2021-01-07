---
title: Eliminar el sitio de raíz de SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768457"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="cc5a3-102">Eliminar el sitio de raíz de SharePoint</span><span class="sxs-lookup"><span data-stu-id="cc5a3-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="cc5a3-103">**No se admite** la eliminación del sitio de raíz de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cc5a3-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="cc5a3-104">Si el sitio de raíz ya se ha eliminado, los usuarios recibirán un error 404 Archivo no encontrado si intentan acceder al sitio en cuestión.</span><span class="sxs-lookup"><span data-stu-id="cc5a3-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="cc5a3-105">Para resolver el problema, restaure el sitio desde el Centro de administración de SharePoint. Para ello, vaya a la página [Sitios eliminados](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true), seleccione el sitio de raíz y haga clic en Restaurar.</span><span class="sxs-lookup"><span data-stu-id="cc5a3-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="cc5a3-106">En lugar de eliminar el sitio de raíz, utilice [reemplazar sitio](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) desde el nuevo Centro de administración de SharePoint una vez que el sitio de raíz haya sido restaurado.</span><span class="sxs-lookup"><span data-stu-id="cc5a3-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="cc5a3-107">Para obtener más información sobre los requisitos, consulte [Modernizar el sitio raíz](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="cc5a3-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>