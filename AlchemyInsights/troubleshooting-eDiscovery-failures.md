---
title: 1490-solución de problemas-errores de exhibición de documentos electrónicos
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277818"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="01fe0-102">Solucionar errores de búsqueda de contenido</span><span class="sxs-lookup"><span data-stu-id="01fe0-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="01fe0-103">¿Tiene problemas con la búsqueda de contenido o la obtención de errores al exportar los resultados de la búsqueda?</span><span class="sxs-lookup"><span data-stu-id="01fe0-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="01fe0-104">Por ejemplo, ¿recibe lo siguiente cuando ejecuta búsquedas?</span><span class="sxs-lookup"><span data-stu-id="01fe0-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="01fe0-105">Errores CS008 o CS012</span><span class="sxs-lookup"><span data-stu-id="01fe0-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="01fe0-106">Errores de tiempo de espera o de servidor ocupado</span><span class="sxs-lookup"><span data-stu-id="01fe0-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="01fe0-107">Se produjo un error en la aplicación</span><span class="sxs-lookup"><span data-stu-id="01fe0-107">Application error occurred</span></span>

<span data-ttu-id="01fe0-108">O bien, al buscar o exportar resultados de un gran número de buzones (más de 100.000 buzones), ¿recibe errores de exportación?</span><span class="sxs-lookup"><span data-stu-id="01fe0-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="01fe0-109">Para estos tipos de errores, vuelva a intentar la búsqueda de las ubicaciones de contenido que han fallado.</span><span class="sxs-lookup"><span data-stu-id="01fe0-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="01fe0-110">Consulte  [este artículo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="01fe0-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="01fe0-111">Si va a exportar más de 100 k buzones, tendrá que usar el siguiente PowerShell para descargar los resultados de la exportación:  [exportar resultados de más de 100 k buzones de correo](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="01fe0-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
