---
title: Herramienta de exportación de exhibición de documentos electrónicos
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814605"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="c1149-102">¿No se puede instalar o ejecutar la herramienta de exportación de exhibición de documentos electrónicos?</span><span class="sxs-lookup"><span data-stu-id="c1149-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="c1149-103">Si no puede instalar o ejecutar la herramienta de exportación de exhibición de documentos electrónicos para descargar los resultados de búsqueda, compruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="c1149-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="c1149-104">El equipo que está usando cumple estos requisitos previos:</span><span class="sxs-lookup"><span data-stu-id="c1149-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="c1149-105">Versiones de 32 o 64 bits de Windows 7 y versiones posteriores</span><span class="sxs-lookup"><span data-stu-id="c1149-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="c1149-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="c1149-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="c1149-107">Un explorador compatible:</span><span class="sxs-lookup"><span data-stu-id="c1149-107">A supported browser:</span></span>

  - <span data-ttu-id="c1149-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c1149-108">Microsoft Edge</span></span>

    <span data-ttu-id="c1149-109">O bien:</span><span class="sxs-lookup"><span data-stu-id="c1149-109">Or</span></span>

  - <span data-ttu-id="c1149-110">Internet Explorer 10 y versiones posteriores</span><span class="sxs-lookup"><span data-stu-id="c1149-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="c1149-111">No se admiten otros exploradores, como Google Chrome y Mozilla Firefox.</span><span class="sxs-lookup"><span data-stu-id="c1149-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="c1149-112">Su organización puede conectarse al punto de conexión de Azure, que **\* es .blob.core.windows.net** (el comodín representa un identificador único para el trabajo de exportación).</span><span class="sxs-lookup"><span data-stu-id="c1149-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="c1149-113">Se le asigna el rol Exportar en el Centro de cumplimiento de seguridad de Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="c1149-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="c1149-114">De forma predeterminada, este rol solo se asigna al grupo de roles administrador de exhibición de documentos electrónicos.</span><span class="sxs-lookup"><span data-stu-id="c1149-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="c1149-115">Vea [Asignar permisos de exhibición de documentos electrónicos.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="c1149-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="c1149-116">Para obtener más información, vea [Exportar resultados de búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="c1149-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="c1149-117">Si exporta más de 100.000 buzones, deberá usar el siguiente Powershell para descargar los resultados de exportación: Exportar resultados de más de [100 mil buzones.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="c1149-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>