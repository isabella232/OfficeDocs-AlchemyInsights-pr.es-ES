---
title: No hay resultados en la búsqueda de contenido
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680664"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="4fa9a-102">No hay resultados en la búsqueda/exportación de contenido</span><span class="sxs-lookup"><span data-stu-id="4fa9a-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="4fa9a-103">Problemas con la búsqueda y las exportaciones de contenido que no devuelven datos puede deberse a ciertos filtros de seguridad de cumplimiento que han sido configurados por un administrador específico y no lo comunican a todos los administradores.</span><span class="sxs-lookup"><span data-stu-id="4fa9a-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="4fa9a-104">Para solucionar esto, compruebe si hay filtros de seguridad de cumplimiento que puedan estar causando esto:</span><span class="sxs-lookup"><span data-stu-id="4fa9a-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="4fa9a-105">Conectarse al centro de seguridad y cumplimiento PowerShell</span><span class="sxs-lookup"><span data-stu-id="4fa9a-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="4fa9a-106">Ejecute el siguiente commandlets:</span><span class="sxs-lookup"><span data-stu-id="4fa9a-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="4fa9a-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="4fa9a-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="4fa9a-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="4fa9a-108">Get-ComplianceSecurityFilter -Organization $org</span></span>