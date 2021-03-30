---
title: Flujo de trabajo no se está iniciando
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403760"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="1a78c-102">Flujo de trabajo no se está iniciando</span><span class="sxs-lookup"><span data-stu-id="1a78c-102">Workflow is not starting</span></span>

- <span data-ttu-id="1a78c-103">Los flujos de trabajo de SharePoint 2010 y SharePoint 2013 no se inician.</span><span class="sxs-lookup"><span data-stu-id="1a78c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="1a78c-104">Si el flujo de trabajo no se inicia, puede haber un problema de servicio temporal en el que los usuarios pueden experimentar retrasos intermitentes con el progreso del flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="1a78c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="1a78c-105">Compruebe el [Panel de estado del servicio](https://admin.microsoft.com/AdminPortal/Home/servicehealth) para ver si su organización está afectada.</span><span class="sxs-lookup"><span data-stu-id="1a78c-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="1a78c-106">Si han pasado más de 24 horas desde que vio por primera vez este problema, registre un vale de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="1a78c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1a78c-107">En muchos casos, ya estamos trabajando en una solución.</span><span class="sxs-lookup"><span data-stu-id="1a78c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1a78c-108">Por favor, dénos al menos 24 horas para completar una solución.</span><span class="sxs-lookup"><span data-stu-id="1a78c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="1a78c-109">Los flujos de trabajo de SharePoint 2010 se retrasaron al inicio.</span><span class="sxs-lookup"><span data-stu-id="1a78c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="1a78c-110">Esto ocurre si el flujo de trabajo se desencadena en lotes grandes.</span><span class="sxs-lookup"><span data-stu-id="1a78c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="1a78c-111">(por ejemplo, cuando se agregan varios elementos a la vez).</span><span class="sxs-lookup"><span data-stu-id="1a78c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="1a78c-112">Los flujos de trabajo no están diseñados para ejecutarse en tiempo real, por lo que un retraso es un comportamiento por diseño.</span><span class="sxs-lookup"><span data-stu-id="1a78c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="1a78c-113">Si el flujo de trabajo es complejo Extensible Object Markup Language (XMOL), la compilación puede ser lenta.</span><span class="sxs-lookup"><span data-stu-id="1a78c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="1a78c-114">Consulte [este](https://support.microsoft.com//kb/3043697) artículo.</span><span class="sxs-lookup"><span data-stu-id="1a78c-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="1a78c-115">Debe simplificar el flujo de trabajo o rediseñar el flujo de trabajo con el tipo de plataforma flujo de trabajo de Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="1a78c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="1a78c-116">Si el historial de flujo de trabajo se ha hecho grande, es posible que desee purgar los elementos o crear una lista de historial nueva.</span><span class="sxs-lookup"><span data-stu-id="1a78c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="1a78c-117">Más información: [Purgar historial de flujos de trabajo](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="1a78c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="1a78c-118">Temas relacionados</span><span class="sxs-lookup"><span data-stu-id="1a78c-118">Related topics</span></span>
<span data-ttu-id="1a78c-119">¿Desea probar Microsoft Flow en SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="1a78c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1a78c-120">Crear flujo</span><span class="sxs-lookup"><span data-stu-id="1a78c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1a78c-121">SharePoint y Flow</span><span class="sxs-lookup"><span data-stu-id="1a78c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
