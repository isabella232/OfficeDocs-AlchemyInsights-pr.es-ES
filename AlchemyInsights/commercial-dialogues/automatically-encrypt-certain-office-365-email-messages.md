---
title: Cifrar automáticamente determinados mensajes de correo electrónico de Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737611"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="10f72-102">Cifrar automáticamente determinados mensajes de correo electrónico de Office 365</span><span class="sxs-lookup"><span data-stu-id="10f72-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="10f72-103">Puede cifrar automáticamente los mensajes que los usuarios envían a determinadas personas u organizaciones externas.</span><span class="sxs-lookup"><span data-stu-id="10f72-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="10f72-104">Para ello, realice los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="10f72-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="10f72-105">En el [Centro de administración de Exchange,](https://outlook.office365.com/ecp/)elija flujo de correo > **reglas**.</span><span class="sxs-lookup"><span data-stu-id="10f72-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="10f72-106">Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar el cifrado de mensajes de Office **365** y la protección de derechos a los mensajes .</span><span class="sxs-lookup"><span data-stu-id="10f72-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="10f72-107">En **Nombre**, escriba un nombre para la regla, como *Cifrar mensajes enviados a DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="10f72-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="10f72-108">En **Aplicar esta regla si**, elija El destinatario > es esta **persona**.</span><span class="sxs-lookup"><span data-stu-id="10f72-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="10f72-109">En la **ventana Seleccionar miembros,** seleccione el nombre de la persona a la que desea que se aplique la regla de cifrado y, a continuación, haga clic en **Agregar**.</span><span class="sxs-lookup"><span data-stu-id="10f72-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="10f72-110">Cuando haya terminado de agregar usuarios, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="10f72-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="10f72-111">Junto al campo **Hacer lo siguiente,** haga clic **en Seleccionar uno**.</span><span class="sxs-lookup"><span data-stu-id="10f72-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="10f72-112">En el **menú desplegable Plantilla RMS,** seleccione **Cifrar** y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="10f72-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="10f72-113">(Si no ve esta opción, significa que el plan no incluye cifrado automático.</span><span class="sxs-lookup"><span data-stu-id="10f72-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="10f72-114">Pero puedes agregarlo!</span><span class="sxs-lookup"><span data-stu-id="10f72-114">But you can add it!)</span></span>
9. <span data-ttu-id="10f72-115">Elija cualquier selección opcional (de una lista de selecciones opcionales que puede realizar en este momento, muchas de las cuales se pueden dejar con la configuración predeterminada para simplificar).</span><span class="sxs-lookup"><span data-stu-id="10f72-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="10f72-116">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="10f72-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="10f72-117">Siempre puede volver y editar esta regla más adelante.</span><span class="sxs-lookup"><span data-stu-id="10f72-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="10f72-118">Para obtener más información acerca de cómo crear reglas de cifrado, vea Definir reglas de flujo de correo para cifrar mensajes de correo [electrónico en Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="10f72-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

