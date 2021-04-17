---
title: Solucionar el error AADSTS9000411 de inicio de sesión en Teams
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822004"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="d91ee-102">Solucionar el error AADSTS9000411 de inicio de sesión en Teams</span><span class="sxs-lookup"><span data-stu-id="d91ee-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="d91ee-103">Al iniciar sesión en Microsoft Teams, es posible que reciba el error siguiente: **Estamos teniendo problemas para iniciar sesión en AADSTS9000411: la solicitud no tiene el formato correcto. El parámetro "login_hint" está duplicado.**</span><span class="sxs-lookup"><span data-stu-id="d91ee-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="d91ee-104">Para solucionar este problema, asegúrese de que sus clientes de Microsoft Teams estén actualizados.</span><span class="sxs-lookup"><span data-stu-id="d91ee-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="d91ee-105">Para más información sobre cómo actualizar el cliente, consulte [Actualizar Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="d91ee-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="d91ee-106">Si, por algún motivo, no puede actualizar el cliente, cerrar sesión en el cliente borrará la mayoría de los datos almacenados en caché.</span><span class="sxs-lookup"><span data-stu-id="d91ee-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="d91ee-107">Sin embargo, si aún tiene problemas después de cerrar sesión o iniciar sesión, salga de Teams y borre la caché de cliente haciendo lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d91ee-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="d91ee-108">Cierre Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d91ee-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="d91ee-109">Vaya a: %appdata%\microsoft\teams y elimine todos los archivos.</span><span class="sxs-lookup"><span data-stu-id="d91ee-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="d91ee-110">Vuelva a abrir Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d91ee-110">Reopen Microsoft Teams.</span></span>
