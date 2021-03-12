---
title: Cifrar automáticamente los mensajes de correo electrónico de Office 365 enviados a determinados dominios
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737588"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="8ab36-102">Cifrar automáticamente los mensajes de correo electrónico de Office 365 enviados a determinados dominios</span><span class="sxs-lookup"><span data-stu-id="8ab36-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="8ab36-103">En el [Centro de administración de Exchange,](https://outlook.office365.com/ecp/)elija flujo de correo > **reglas**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="8ab36-104">Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar el cifrado de mensajes de Office **365** y la protección de derechos a los mensajes .</span><span class="sxs-lookup"><span data-stu-id="8ab36-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="8ab36-105">En **Nombre**, escriba un nombre para la regla, como *Cifrar mensajes enviados* a contoso.com .</span><span class="sxs-lookup"><span data-stu-id="8ab36-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="8ab36-106">En **Aplicar esta regla si**, elija El destinatario > dominio **es**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="8ab36-107">Escriba el nombre del dominio, como **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="8ab36-108">Haga clic **en el icono Agregar (+)** y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="8ab36-109">Junto al campo **Hacer lo siguiente,** haga clic **en Seleccionar uno**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="8ab36-110">En el **menú desplegable Plantilla RMS,** seleccione **Cifrar** y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="8ab36-111">(Si no ve esta opción, significa que el plan no incluye cifrado automático.</span><span class="sxs-lookup"><span data-stu-id="8ab36-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="8ab36-112">Pero puedes agregarlo!</span><span class="sxs-lookup"><span data-stu-id="8ab36-112">But you can add it!)</span></span>
9. <span data-ttu-id="8ab36-113">Elija cualquier selección opcional (de una lista de selecciones opcionales que puede realizar en este momento, muchas de las cuales se pueden dejar con la configuración predeterminada para simplificar).</span><span class="sxs-lookup"><span data-stu-id="8ab36-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="8ab36-114">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="8ab36-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8ab36-115">Siempre puede volver y editar esta regla más adelante.</span><span class="sxs-lookup"><span data-stu-id="8ab36-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="8ab36-116">Para obtener más información sobre cómo crear reglas de cifrado, vea Definir reglas de flujo de correo [para cifrar mensajes de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="8ab36-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>