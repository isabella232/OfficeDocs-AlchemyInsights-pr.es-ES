---
title: Limitación de SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773864"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="31fc1-102">Limitación de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="31fc1-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="31fc1-103">**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="31fc1-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="31fc1-104">**503 el servidor está ocupado error**</span><span class="sxs-lookup"><span data-stu-id="31fc1-104">**503 server is busy error**</span></span>

<span data-ttu-id="31fc1-105">Es posible que los usuarios reciban un error de un servidor de 503 al intentar navegar a sitios de SharePoint o de OneDrive.</span><span class="sxs-lookup"><span data-stu-id="31fc1-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="31fc1-106">Este error puede deberse a una limitación en el servicio de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="31fc1-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="31fc1-107">SharePoint Online utiliza limitación para mantener un rendimiento óptimo y la confiabilidad del servicio SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="31fc1-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="31fc1-108">La limitación restringe el número de acciones de usuario o llamadas simultáneas (mediante script o código) para evitar el uso excesivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="31fc1-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="31fc1-109">Para obtener más información sobre la limitación de peticiones, consulte [limitar o bloqueado en SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="31fc1-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="31fc1-110">Si cree que este error no está relacionado con la limitación, puede comprobar si hay mantenimiento activo en su espacio empresarial desplazándose al [centro de mensajes](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="31fc1-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="31fc1-111">Por último, asegúrese de visitar la página de [Estado del servicio](https://portal.office.com/adminportal/home#/servicehealth) para comprobar si hay algún asesor o incidente que pueda producirse.</span><span class="sxs-lookup"><span data-stu-id="31fc1-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

