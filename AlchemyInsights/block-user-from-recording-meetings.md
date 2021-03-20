---
title: Bloquear al usuario para que no grabe reuniones
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897977"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="bb069-102">Bloquear al usuario para que no grabe reuniones</span><span class="sxs-lookup"><span data-stu-id="bb069-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="bb069-103">Si necesitas impedir o **bloquear que** usuarios específicos graben reuniones de Teams, puedes hacerlo a través de la configuración de la directiva de reunión de Teams.</span><span class="sxs-lookup"><span data-stu-id="bb069-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="bb069-104">En el Centro de administración de Microsoft Teams, desactiva la configuración Permitir grabación **en** la nube en la directiva de reunión asignada a ese usuario.</span><span class="sxs-lookup"><span data-stu-id="bb069-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="bb069-105">Para obtener más información, vea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="bb069-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="bb069-106">Para validar si un usuario específico tiene permiso o no para grabar reuniones de Teams, use el diagnóstico de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="bb069-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="bb069-107">Ejecute una nueva consulta de soporte técnico y escriba **Diag: Meeting Recording:** el diagnóstico comprobará la configuración de directiva del usuario especificado y determinará su configuración de directiva.</span><span class="sxs-lookup"><span data-stu-id="bb069-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="bb069-108">Recuerde que la nueva configuración de directiva puede tardar un par de horas en tener efecto, por lo que si acaba de realizar un cambio, espere unas horas antes de volver a ejecutar el diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="bb069-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="bb069-109">Para obtener más información, revise [Activar o desactivar la grabación en la nube.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="bb069-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
