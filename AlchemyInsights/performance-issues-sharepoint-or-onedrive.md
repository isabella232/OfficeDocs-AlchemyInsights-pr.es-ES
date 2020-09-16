---
title: 'Problemas de rendimiento: SharePoint o OneDrive'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771918"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="64fbc-102">SharePoint o OneDrive es lento, inaccesible o no disponible para varios usuarios</span><span class="sxs-lookup"><span data-stu-id="64fbc-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="64fbc-103">SharePoint o OneDrive puede ser lento, inaccesible o no disponible, o puede mostrar los errores servicio no disponible o 503, por varios motivos:</span><span class="sxs-lookup"><span data-stu-id="64fbc-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="64fbc-104">Si el sitio de SharePoint o de OneDrive es lento o se retrasa para varios usuarios, es posible que haya un problema de servicio temporal en el que los usuarios experimenten retrasos intermitentes o errores de navegación al obtener acceso a sitios de SharePoint o contenido de OneDrive.</span><span class="sxs-lookup"><span data-stu-id="64fbc-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="64fbc-105">Consulte el [panel de estado del servicio](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para comprobar si la organización está afectada.</span><span class="sxs-lookup"><span data-stu-id="64fbc-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="64fbc-106">Es posible que los usuarios reciban un error de un *servidor de 503* al intentar navegar a sitios de SharePoint o de OneDrive.</span><span class="sxs-lookup"><span data-stu-id="64fbc-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="64fbc-107">Este error puede deberse a una limitación en el servicio de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="64fbc-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="64fbc-108">SharePoint Online utiliza limitación para mantener un rendimiento óptimo y la confiabilidad del servicio SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="64fbc-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="64fbc-109">La limitación restringe el número de acciones de usuario o llamadas simultáneas (mediante script o código) para evitar el uso excesivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="64fbc-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="64fbc-110">Para obtener más información sobre la limitación de peticiones, consulte [limitar o bloqueado en SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="64fbc-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="64fbc-111">Si experimenta un rendimiento lento con un sitio o página de SharePoint **clásico** o **moderno** , use la [herramienta de diagnóstico de páginas](https://aka.ms/perftool) para analizar las páginas.</span><span class="sxs-lookup"><span data-stu-id="64fbc-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="64fbc-112">Si sigue experimentando un rendimiento lento general, revise los recursos que se encuentra en la parte inferior de este artículo: [Introducción al ajuste del rendimiento de SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334) .</span><span class="sxs-lookup"><span data-stu-id="64fbc-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  