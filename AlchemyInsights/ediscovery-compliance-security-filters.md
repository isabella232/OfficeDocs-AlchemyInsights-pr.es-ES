---
title: No se devolvieron resultados durante la búsqueda o exportación de contenido
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
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666666"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="bee7d-102">No se devolvieron resultados durante la búsqueda o exportación de contenido</span><span class="sxs-lookup"><span data-stu-id="bee7d-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="bee7d-103">Si experimenta problemas con los siguientes escenarios de exhibición de documentos electrónicos:</span><span class="sxs-lookup"><span data-stu-id="bee7d-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="bee7d-104">La búsqueda y la exportación de contenido no devuelve datos o datos inesperados</span><span class="sxs-lookup"><span data-stu-id="bee7d-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="bee7d-105">error de búsqueda o exportación de eDiscovery</span><span class="sxs-lookup"><span data-stu-id="bee7d-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="bee7d-106">Esto puede deberse a ciertos filtros de seguridad de cumplimiento que fueron configurados por un administrador específico y que no se han comunicado a todos los administradores.</span><span class="sxs-lookup"><span data-stu-id="bee7d-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="bee7d-107">Para solucionar esto, compruebe si hay filtros de seguridad de cumplimiento que puedan causar estos problemas:</span><span class="sxs-lookup"><span data-stu-id="bee7d-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="bee7d-108">Conectarse al centro de seguridad y cumplimiento PowerShell</span><span class="sxs-lookup"><span data-stu-id="bee7d-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="bee7d-109">Ejecute el siguiente commandlets:</span><span class="sxs-lookup"><span data-stu-id="bee7d-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="bee7d-110">Para obtener información adicional sobre los filtros de seguridad de cumplimiento, consulte [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="bee7d-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
