---
title: Búsqueda de contenido sin resultados
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816865"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="a42a5-102">Sin resultados de búsqueda o exportación de contenido</span><span class="sxs-lookup"><span data-stu-id="a42a5-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="a42a5-103">Los problemas con la búsqueda o las exportaciones de contenido que no devuelven datos pueden deberse a cierto filtro de seguridad de cumplimiento configurado por un administrador específico y a no comunicarlo a todos los administradores.</span><span class="sxs-lookup"><span data-stu-id="a42a5-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="a42a5-104">Para resolver esto, compruebe si hay filtros de seguridad de cumplimiento que puedan estar causando esto:</span><span class="sxs-lookup"><span data-stu-id="a42a5-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="a42a5-105">Conectarse a PowerShell del Centro de seguridad y cumplimiento</span><span class="sxs-lookup"><span data-stu-id="a42a5-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="a42a5-106">Ejecute los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="a42a5-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="a42a5-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="a42a5-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="a42a5-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="a42a5-108">Get-ComplianceSecurityFilter -Organization $org</span></span>