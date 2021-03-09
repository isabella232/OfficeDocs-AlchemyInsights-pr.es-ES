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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530226"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="d8a87-102">Ejemplo de directiva de datos adjuntos seguros de Microsoft Defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="d8a87-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="d8a87-103">Estas opciones de configuración habilitan una directiva denominada *Sin* retrasos que entrega mensajes inmediatamente y, a continuación, vuelve a adjuntar datos adjuntos después de examinarse:</span><span class="sxs-lookup"><span data-stu-id="d8a87-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="d8a87-104">**Nombre:** sin retrasos</span><span class="sxs-lookup"><span data-stu-id="d8a87-104">**Name**: No delays</span></span>
- <span data-ttu-id="d8a87-105">**Descripción:** entrega los mensajes inmediatamente y vuelve a adjuntar los datos adjuntos después del examen.</span><span class="sxs-lookup"><span data-stu-id="d8a87-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="d8a87-106">**Respuesta:** seleccione la **opción Entrega** dinámica.</span><span class="sxs-lookup"><span data-stu-id="d8a87-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="d8a87-107">Para obtener más información, vea [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="d8a87-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="d8a87-108">**Sección** Redirigir datos adjuntos: seleccione la opción Habilitar redireccionamiento **y,** a continuación, escriba la dirección de correo electrónico de su administrador global de Microsoft 365, administrador de seguridad o analista de seguridad que investigará datos adjuntos malintencionados.</span><span class="sxs-lookup"><span data-stu-id="d8a87-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="d8a87-109">**Sección Aplicado a:** Seleccione **El dominio de destinatario es** y, a continuación, seleccione su dominio.</span><span class="sxs-lookup"><span data-stu-id="d8a87-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="d8a87-110">Seleccione **agregar** y, a continuación, **seleccione Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="d8a87-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="d8a87-111">Una vez que haya terminado, seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="d8a87-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="d8a87-112">Para obtener más información, vea [Datos adjuntos seguros en Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="d8a87-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
