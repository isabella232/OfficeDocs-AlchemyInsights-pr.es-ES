---
title: Buscar la dirección IP en el registro de auditoría
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465003"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="3da27-102">Buscar la dirección IP en el registro de auditoría</span><span class="sxs-lookup"><span data-stu-id="3da27-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="3da27-103">La dirección IP que corresponde a una actividad realizada por un usuario o administrador se muestra en los registros de auditoría.</span><span class="sxs-lookup"><span data-stu-id="3da27-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="3da27-104">También se registra la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="3da27-104">The client information is also logged.</span></span> <span data-ttu-id="3da27-105">A continuación se muestra cómo identificar la dirección IP:</span><span class="sxs-lookup"><span data-stu-id="3da27-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="3da27-106">Vaya al Centro [de seguridad y cumplimiento de Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="3da27-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="3da27-107">Seleccione **Búsqueda de registro** de auditoría de  >  **[búsqueda](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="3da27-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="3da27-108">Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora.</span><span class="sxs-lookup"><span data-stu-id="3da27-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="3da27-109">Si esta característica no está habilitada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.</span><span class="sxs-lookup"><span data-stu-id="3da27-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="3da27-110">Si está interesado en una actividad específica, selecciónelo en la **lista** Actividades; de lo contrario, de forma predeterminada, se devolverán todas las actividades para el usuario seleccionado.</span><span class="sxs-lookup"><span data-stu-id="3da27-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="3da27-111">Tenga en cuenta que es posible que ciertas actividades no estén disponibles para su selección en el **menú** Actividades; sin embargo, esos elementos de auditoría se devolverán si se selecciona Mostrar resultados **para** todas las actividades (configuración predeterminada).</span><span class="sxs-lookup"><span data-stu-id="3da27-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="3da27-112">Especifique el intervalo de fechas y, en el **campo Usuarios,** seleccione el nombre de usuario del usuario que desea investigar.</span><span class="sxs-lookup"><span data-stu-id="3da27-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="3da27-113">Seleccione **Buscar**.</span><span class="sxs-lookup"><span data-stu-id="3da27-113">Select **Search**.</span></span> <span data-ttu-id="3da27-114">Las actividades aparecen en **Resultados**.</span><span class="sxs-lookup"><span data-stu-id="3da27-114">The activities appear under **Results**.</span></span> <span data-ttu-id="3da27-115">Puede ver la dirección IP de cada actividad.</span><span class="sxs-lookup"><span data-stu-id="3da27-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="3da27-116">Para ver detalles, seleccione una actividad y, a continuación, **seleccione Más información**.</span><span class="sxs-lookup"><span data-stu-id="3da27-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="3da27-117">Para obtener más información, vea Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="3da27-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>