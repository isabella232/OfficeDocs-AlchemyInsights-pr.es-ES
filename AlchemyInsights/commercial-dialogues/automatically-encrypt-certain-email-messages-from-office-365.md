---
title: Cifrar automáticamente determinados mensajes de correo electrónico de office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737612"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="9a572-102">Cifrar automáticamente determinados mensajes de correo electrónico de office 365</span><span class="sxs-lookup"><span data-stu-id="9a572-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="9a572-103">En el [Centro de administración de Exchange,](https://outlook.office365.com/ecp/)elija flujo de correo > **reglas**.</span><span class="sxs-lookup"><span data-stu-id="9a572-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9a572-104">Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar el cifrado de mensajes de Office **365** y la protección de derechos a los mensajes .</span><span class="sxs-lookup"><span data-stu-id="9a572-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9a572-105">En **Nombre**, escriba un nombre para la regla, como *Cifrar todos los mensajes*.</span><span class="sxs-lookup"><span data-stu-id="9a572-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="9a572-106">En **Aplicar esta regla si**, elija **[Aplicar a todos los mensajes]**.</span><span class="sxs-lookup"><span data-stu-id="9a572-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="9a572-107">Junto al campo **Hacer lo siguiente,** haga clic **en Seleccionar uno**.</span><span class="sxs-lookup"><span data-stu-id="9a572-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="9a572-108">En el **menú desplegable Plantilla RMS,** seleccione **Cifrar** y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="9a572-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9a572-109">(Si no ve esta opción, significa que el plan no incluye cifrado automático.</span><span class="sxs-lookup"><span data-stu-id="9a572-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9a572-110">Pero puedes agregarlo!</span><span class="sxs-lookup"><span data-stu-id="9a572-110">But you can add it!)</span></span>
7. <span data-ttu-id="9a572-111">Active la **casilla Auditar esta regla con** el nivel de gravedad y, a continuación, seleccione el nivel deseado.</span><span class="sxs-lookup"><span data-stu-id="9a572-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="9a572-112">Si su empresa tiene obligaciones contractuales para enviar todos los correos electrónicos cifrados, le recomiendo establecer el nivel en **Alto**.</span><span class="sxs-lookup"><span data-stu-id="9a572-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="9a572-113">En **Elegir un modelo para esta regla,** haga clic en **Exigir**.</span><span class="sxs-lookup"><span data-stu-id="9a572-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="9a572-114">Elija cualquier selección opcional (de una lista de selecciones opcionales que puede realizar en este momento, muchas de las cuales se pueden dejar con la configuración predeterminada para simplificar).</span><span class="sxs-lookup"><span data-stu-id="9a572-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9a572-115">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="9a572-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9a572-116">Siempre puede volver y editar esta regla más adelante.</span><span class="sxs-lookup"><span data-stu-id="9a572-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9a572-117">Para obtener más información sobre cómo crear reglas de cifrado, vea Definir reglas de flujo de correo [para cifrar mensajes de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="9a572-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

