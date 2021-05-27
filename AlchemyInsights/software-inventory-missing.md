---
title: El inventario de software no se encuentra o no es exacto.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658059"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="4923d-102">El inventario de software no se encuentra o no es exacto.</span><span class="sxs-lookup"><span data-stu-id="4923d-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="4923d-103">El inventario de software en la Administración de amenazas y vulnerabilidades (TVM) es una lista de software conocido en su organización con Enumeraciones de plataformas comunes (CPE) oficiales.</span><span class="sxs-lookup"><span data-stu-id="4923d-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="4923d-104">Los productos de software sin CPE oficiales no tienen vulnerabilidades publicadas.</span><span class="sxs-lookup"><span data-stu-id="4923d-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="4923d-105">El inventario también incluye detalles como el nombre del proveedor, el número de debilidades, las amenazas y el número de dispositivos expuestos.</span><span class="sxs-lookup"><span data-stu-id="4923d-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="4923d-106">Los cambios del software en los dispositivos normalmente se reflejan en los portales de seguridad en dos horas.</span><span class="sxs-lookup"><span data-stu-id="4923d-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="4923d-107">Sin embargo, a veces pueden tardar más.</span><span class="sxs-lookup"><span data-stu-id="4923d-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="4923d-108">Actualmente, no hay ninguna forma de forzar la sincronización: es una evaluación continua.</span><span class="sxs-lookup"><span data-stu-id="4923d-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="4923d-109">Si realizó un cambio de software y el cambio no se refleja con precisión en la TVM después de 5 horas, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="4923d-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="4923d-110">Compruebe la sección de evidencia del software para comprender cómo fue detectado el software.</span><span class="sxs-lookup"><span data-stu-id="4923d-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="4923d-111">Asegúrese de que el software sea compatible.</span><span class="sxs-lookup"><span data-stu-id="4923d-111">Make sure that the software is supported.</span></span> <span data-ttu-id="4923d-112">Es posible que el software solo sea visible a nivel del dispositivo, incluso si actualmente no es compatible con la Administración de amenazas y vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="4923d-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="4923d-113">Sin embargo, solo están disponibles los datos limitados.</span><span class="sxs-lookup"><span data-stu-id="4923d-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="4923d-114">Para obtener información sobre cómo informar la inexactitud desde el portal, consulte [Informar inexactitud](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="4923d-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="4923d-115">**Nota**: Informar de una inexactitud desde el portal MDE es un canal una sola vía para la ingeniería.</span><span class="sxs-lookup"><span data-stu-id="4923d-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="4923d-116">Si el problema es urgente, abra un vale de soporte.</span><span class="sxs-lookup"><span data-stu-id="4923d-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="4923d-117">Para obtener más información, vea [Inventario de software: Administración de amenazas y vulnerabilidades](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="4923d-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>