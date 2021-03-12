---
title: Impedir que los mensajes se muevan al archivo automáticamente
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737668"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="68cb5-102">Impedir que los mensajes se muevan al archivo automáticamente</span><span class="sxs-lookup"><span data-stu-id="68cb5-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="68cb5-103">Si usa una directiva de retención, puede cambiar la antigüedad de retención en esa directiva para impedir que los mensajes se archiven automáticamente.</span><span class="sxs-lookup"><span data-stu-id="68cb5-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="68cb5-104">A continuación se describe cómo:</span><span class="sxs-lookup"><span data-stu-id="68cb5-104">Here's how:</span></span>

1. <span data-ttu-id="68cb5-105">En el [Centro de administración de Exchange,](https://go.microsoft.com/fwlink/?linkid=2059104)elija **etiquetas de retención de administración** de  >  **cumplimiento.**</span><span class="sxs-lookup"><span data-stu-id="68cb5-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="68cb5-106">Busque la etiqueta de retención Mover a archivo.</span><span class="sxs-lookup"><span data-stu-id="68cb5-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="68cb5-107">En la etiqueta de retención, cambie el período de retención (período de archivo) a **Nunca** para impedir que los elementos se archiven automáticamente mediante una directiva de retención.</span><span class="sxs-lookup"><span data-stu-id="68cb5-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="68cb5-108">Esto cambiará la configuración de archivo de todos los buzones con esta etiqueta de retención aplicada a ellos.</span><span class="sxs-lookup"><span data-stu-id="68cb5-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
