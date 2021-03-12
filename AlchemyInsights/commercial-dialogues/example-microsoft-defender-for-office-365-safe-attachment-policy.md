---
title: Ejemplo de directiva de datos adjuntos seguros de Microsoft Defender para Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737572"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="6ef62-102">Ejemplo de directiva de datos adjuntos seguros de Microsoft Defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="6ef62-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="6ef62-103">Estas opciones de configuración habilitan una directiva denominada *Sin* retrasos que entrega mensajes inmediatamente y, a continuación, vuelve a adjuntar datos adjuntos después de examinarse:</span><span class="sxs-lookup"><span data-stu-id="6ef62-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="6ef62-104">**Nombre:** sin retrasos</span><span class="sxs-lookup"><span data-stu-id="6ef62-104">**Name**: No delays</span></span>
- <span data-ttu-id="6ef62-105">**Descripción:** entrega los mensajes inmediatamente y vuelve a adjuntar los datos adjuntos después del examen.</span><span class="sxs-lookup"><span data-stu-id="6ef62-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="6ef62-106">**Respuesta:** seleccione la **opción Entrega** dinámica.</span><span class="sxs-lookup"><span data-stu-id="6ef62-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="6ef62-107">Para obtener más información, vea [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="6ef62-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="6ef62-108">**Sección** Redirigir datos adjuntos: seleccione la opción Habilitar redireccionamiento **y,** a continuación, escriba la dirección de correo electrónico de su administrador global de Microsoft 365, administrador de seguridad o analista de seguridad que investigará datos adjuntos malintencionados.</span><span class="sxs-lookup"><span data-stu-id="6ef62-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="6ef62-109">**Sección Aplicado a:** Seleccione **El dominio de destinatario es** y, a continuación, seleccione su dominio.</span><span class="sxs-lookup"><span data-stu-id="6ef62-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="6ef62-110">Seleccione **agregar** y, a continuación, **seleccione Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="6ef62-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="6ef62-111">Una vez que haya terminado, seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="6ef62-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="6ef62-112">Para obtener más información, vea [Datos adjuntos seguros en Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="6ef62-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
