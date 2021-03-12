---
title: Corregir directiva de inquilino (invalidación de acción)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737540"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="fc6db-102">Corregir directiva de inquilino (invalidación de acción)</span><span class="sxs-lookup"><span data-stu-id="fc6db-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="fc6db-103">Una directiva contra correo no deseado en el inquilino afectó a este mensaje.</span><span class="sxs-lookup"><span data-stu-id="fc6db-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="fc6db-104">Para revisar la directiva, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="fc6db-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="fc6db-105">Vaya al Centro de seguridad y & seguridad de [Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)y, a continuación, vaya a **Directiva** de administración de amenazas  >    >  [contra correo no deseado.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="fc6db-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="fc6db-106">Compruebe si el **origen de directiva** indica lo  **siguiente: Add-Xheader/ModifySubject/Redirect/Delete/No action/ CC message**</span><span class="sxs-lookup"><span data-stu-id="fc6db-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="fc6db-107">Si es así, en la **pestaña** Personalizado, compruebe la configuración de la directiva que afectó al mensaje.</span><span class="sxs-lookup"><span data-stu-id="fc6db-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="fc6db-108">Es posible que  la configuración estándar aplicada a todos los clientes de Exchange Online Protection afectara al mensaje.</span><span class="sxs-lookup"><span data-stu-id="fc6db-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="fc6db-109">Para obtener más información sobre cómo configurar directivas de filtro de correo no deseado, vea [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="fc6db-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
