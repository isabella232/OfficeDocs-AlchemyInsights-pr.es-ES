---
title: Leer los registros de auditoría para eventos eliminados
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464860"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="11fec-102">Leer los registros de auditoría para eventos eliminados</span><span class="sxs-lookup"><span data-stu-id="11fec-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="11fec-103">Este es el modo de hacerlo:</span><span class="sxs-lookup"><span data-stu-id="11fec-103">Here's how to do this:</span></span>

1. <span data-ttu-id="11fec-104">Vaya al Centro [de seguridad y cumplimiento de Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="11fec-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="11fec-105">Seleccione **Búsqueda de registro** de auditoría de  >  [**búsqueda**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="11fec-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="11fec-106">Si ve un aviso de que necesita activar la característica, adelante y encándala ahora.</span><span class="sxs-lookup"><span data-stu-id="11fec-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="11fec-107">Si la característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.</span><span class="sxs-lookup"><span data-stu-id="11fec-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="11fec-108">Seleccione **Actividades** y, a continuación, busque **Las actividades del buzón de Exchange**.</span><span class="sxs-lookup"><span data-stu-id="11fec-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="11fec-109">Seleccione las **opciones Mensajes eliminados de la carpeta Elementos eliminados** y **Mensajes movidos a la carpeta Elementos** eliminados.</span><span class="sxs-lookup"><span data-stu-id="11fec-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="11fec-110">Cuando haya terminado, haga clic fuera del panel para minimizar el **panel** Actividades.</span><span class="sxs-lookup"><span data-stu-id="11fec-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="11fec-111">Especifique el intervalo de fechas y, a continuación, en el cuadro **Usuarios,** seleccione el nombre de usuario del usuario que desea investigar.</span><span class="sxs-lookup"><span data-stu-id="11fec-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="11fec-112">Puede seleccionar más de un usuario a la vez.</span><span class="sxs-lookup"><span data-stu-id="11fec-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="11fec-113">Seleccione **Buscar**.</span><span class="sxs-lookup"><span data-stu-id="11fec-113">Select **Search**.</span></span> <span data-ttu-id="11fec-114">Las actividades aparecen en **Resultados**.</span><span class="sxs-lookup"><span data-stu-id="11fec-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="11fec-115">Para ver los detalles, seleccione una actividad y, a continuación, **seleccione Más información**.</span><span class="sxs-lookup"><span data-stu-id="11fec-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="11fec-116">Se muestra información adicional sobre el elemento eliminado, como la línea de asunto y la ubicación del elemento cuando se eliminó, en el **campo AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="11fec-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="11fec-117">No puede restaurar elementos eliminados con la característica de registro de auditoría.</span><span class="sxs-lookup"><span data-stu-id="11fec-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="11fec-118">Para restaurar elementos eliminados, vea [Recuperar elementos eliminados o correo electrónico en Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="11fec-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="11fec-119">Para obtener más información, [vea Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="11fec-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
