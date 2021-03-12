---
title: Directiva de conexión de corrección
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737830"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="d53e1-102">Directiva de conexión de corrección</span><span class="sxs-lookup"><span data-stu-id="d53e1-102">Fix connection policy</span></span>

<span data-ttu-id="d53e1-103">El correo electrónico se marcó como seguro y se entregó a la bandeja de entrada del usuario porque la dirección IP de envío estaba marcada como segura en la directiva de filtro de conexión.</span><span class="sxs-lookup"><span data-stu-id="d53e1-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="d53e1-104">Para revisar la directiva, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d53e1-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="d53e1-105">Vaya al Centro de seguridad y & seguridad de [Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)y, a continuación, vaya a **Directiva** de administración de amenazas  >    >  [contra correo no deseado.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="d53e1-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="d53e1-106">En la **pestaña Personalizado,** seleccione la **directiva de filtro de conexión** y, a continuación, seleccione Editar **directiva**.</span><span class="sxs-lookup"><span data-stu-id="d53e1-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="d53e1-107">Revise la **lista de direcciones IP** permitidos.</span><span class="sxs-lookup"><span data-stu-id="d53e1-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="d53e1-108">Vea si **la lista segura** está habilitada.</span><span class="sxs-lookup"><span data-stu-id="d53e1-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d53e1-109">Microsoft se suscribe a fuentes de terceros de remitentes de confianza.</span><span class="sxs-lookup"><span data-stu-id="d53e1-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="d53e1-110">Si **la lista segura** está habilitada, estos remitentes de confianza no se marcan erróneamente como correo no deseado.</span><span class="sxs-lookup"><span data-stu-id="d53e1-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="d53e1-111">Te recomiendo seleccionar esta opción, ya que reducirá el número de falsos positivos (correo bueno que se clasifica como correo no deseado) que recibes.</span><span class="sxs-lookup"><span data-stu-id="d53e1-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
