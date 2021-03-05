---
title: Buscar eventos realizados en reglas de bandeja de entrada
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465000"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="71c0b-102">Buscar eventos realizados en reglas de bandeja de entrada</span><span class="sxs-lookup"><span data-stu-id="71c0b-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="71c0b-103">Cuando se crean, cambian o eliminan reglas de la bandeja de entrada, los eventos se registran en el registro de auditoría.</span><span class="sxs-lookup"><span data-stu-id="71c0b-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="71c0b-104">Este es el modo de revisarlos:</span><span class="sxs-lookup"><span data-stu-id="71c0b-104">Here's how to review them:</span></span>

1. <span data-ttu-id="71c0b-105">Vaya al Centro [de seguridad y cumplimiento de Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="71c0b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="71c0b-106">Seleccione Buscar > registro de auditoría.</span><span class="sxs-lookup"><span data-stu-id="71c0b-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="71c0b-107">Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora.</span><span class="sxs-lookup"><span data-stu-id="71c0b-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="71c0b-108">Si esta característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.</span><span class="sxs-lookup"><span data-stu-id="71c0b-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="71c0b-109">Seleccione el campo Actividades y busque las actividades del buzón de Exchange y, a continuación, New-InboxRule Crear regla de bandeja de entrada desde Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="71c0b-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="71c0b-110">Cuando haya terminado, haga clic fuera del panel para minimizar el panel Actividades.</span><span class="sxs-lookup"><span data-stu-id="71c0b-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="71c0b-111">Especifique el intervalo de fechas y, a continuación, en el campo Usuarios, seleccione el nombre de usuario del usuario que desea investigar.</span><span class="sxs-lookup"><span data-stu-id="71c0b-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="71c0b-112">Puede seleccionar más de un usuario a la vez.</span><span class="sxs-lookup"><span data-stu-id="71c0b-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="71c0b-113">Seleccione Buscar.</span><span class="sxs-lookup"><span data-stu-id="71c0b-113">Select Search.</span></span> <span data-ttu-id="71c0b-114">Las actividades aparecen en Resultados.</span><span class="sxs-lookup"><span data-stu-id="71c0b-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="71c0b-115">Para ver detalles, seleccione una actividad y, a continuación, seleccione Más información.</span><span class="sxs-lookup"><span data-stu-id="71c0b-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="71c0b-116">En la sección Parámetros, puede ver el nombre de la regla, las condiciones establecidas y las acciones que realizará la regla.</span><span class="sxs-lookup"><span data-stu-id="71c0b-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="71c0b-117">Para obtener más información, vea Search the Office 365 audit log to troubleshoot common scenarios.</span><span class="sxs-lookup"><span data-stu-id="71c0b-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>