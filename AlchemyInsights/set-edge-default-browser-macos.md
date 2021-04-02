---
title: Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo con macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426884"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="4e310-102">Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo con macOS</span><span class="sxs-lookup"><span data-stu-id="4e310-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="4e310-103">Use uno de estos dos métodos para establecer Microsoft Edge como explorador web predeterminado:</span><span class="sxs-lookup"><span data-stu-id="4e310-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="4e310-104">Método 1: instale una imagen de macOS donde Microsoft Edge ya se haya establecido como explorador predeterminado.</span><span class="sxs-lookup"><span data-stu-id="4e310-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="4e310-105">Método 2: establezca la directiva Default DomainSettingEnabled para que se pida al usuario que establezca Microsoft Edge como explorador predeterminado.</span><span class="sxs-lookup"><span data-stu-id="4e310-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="4e310-106">Cualquiera de los métodos permite a los usuarios cambiar el explorador predeterminado.</span><span class="sxs-lookup"><span data-stu-id="4e310-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="4e310-107">Por este motivo, le recomendamos que implemente la directiva Default SettingEnabled, incluso si ha usado el método 1.</span><span class="sxs-lookup"><span data-stu-id="4e310-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="4e310-108">Si un usuario cambia el explorador predeterminado después de implementar la directiva, la directiva le pedirá que vuelva a establecer el explorador predeterminado en Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4e310-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
