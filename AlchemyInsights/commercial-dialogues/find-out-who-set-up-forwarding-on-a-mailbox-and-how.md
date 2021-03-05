---
title: Descubra quién configura el reenvío en un buzón y cómo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464872"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="fcb11-102">Descubra quién configura el reenvío en un buzón y cómo</span><span class="sxs-lookup"><span data-stu-id="fcb11-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="fcb11-103">Si se estableció el reenvío externo en un buzón de correo, la actividad se auditará como parte del cmdlet Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="fcb11-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="fcb11-104">Este es el modo de encontrar la actividad en el registro de auditoría:</span><span class="sxs-lookup"><span data-stu-id="fcb11-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="fcb11-105">Vaya al Centro [de seguridad y cumplimiento de Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="fcb11-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="fcb11-106">Seleccione **Búsqueda de registro** de auditoría de >  **búsqueda**.</span><span class="sxs-lookup"><span data-stu-id="fcb11-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="fcb11-107">Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora.</span><span class="sxs-lookup"><span data-stu-id="fcb11-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="fcb11-108">Si esta característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.</span><span class="sxs-lookup"><span data-stu-id="fcb11-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="fcb11-109">Asegúrese de que **el campo** Actividades está establecido en **Mostrar resultados para todas las actividades** (valor predeterminado).</span><span class="sxs-lookup"><span data-stu-id="fcb11-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="fcb11-110">Especifique el intervalo de fechas.</span><span class="sxs-lookup"><span data-stu-id="fcb11-110">Specify the date range.</span></span> <span data-ttu-id="fcb11-111">No es necesario especificar un nombre de usuario.</span><span class="sxs-lookup"><span data-stu-id="fcb11-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="fcb11-112">Seleccione **Buscar**.</span><span class="sxs-lookup"><span data-stu-id="fcb11-112">Select **Search**.</span></span> <span data-ttu-id="fcb11-113">Las actividades aparecen en **Resultados**.</span><span class="sxs-lookup"><span data-stu-id="fcb11-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="fcb11-114">Seleccione **Filtrar resultados** y, a continuación, **escriba Set-mailbox** en el **campo Filtro** de actividad.</span><span class="sxs-lookup"><span data-stu-id="fcb11-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="fcb11-115">Esto devuelve todas **las actividades set-mailbox.**</span><span class="sxs-lookup"><span data-stu-id="fcb11-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="fcb11-116">Para ver los detalles, seleccione una actividad y, a continuación, **seleccione Más información**.</span><span class="sxs-lookup"><span data-stu-id="fcb11-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="fcb11-117">En **Parámetros,** puede ver la dirección de correo electrónico de reenvío que se estableció en el buzón.</span><span class="sxs-lookup"><span data-stu-id="fcb11-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="fcb11-118">UserID **representa** el usuario que configura el reenvío externo en el buzón.</span><span class="sxs-lookup"><span data-stu-id="fcb11-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="fcb11-119">Para obtener más información, [vea Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="fcb11-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>