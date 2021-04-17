---
title: Faltan o no se actualizan eventos del calendario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819984"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="f3b80-102">Faltan o no se actualizan eventos del calendario</span><span class="sxs-lookup"><span data-stu-id="f3b80-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="f3b80-103">Si faltan elementos del calendario o no se actualizan, comience por revisar el recuento de elementos en las propiedades de la carpeta Calendario en Outlook:</span><span class="sxs-lookup"><span data-stu-id="f3b80-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="f3b80-104">Haga clic con el botón derecho en la carpeta **Calendario** del usuario afectado y seleccione **Propiedades**.</span><span class="sxs-lookup"><span data-stu-id="f3b80-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="f3b80-105">Seleccione la pestaña **Sincronización**.</span><span class="sxs-lookup"><span data-stu-id="f3b80-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="f3b80-106">Si el número de elementos no es el mismo en la carpeta Server y la carpeta Offline:</span><span class="sxs-lookup"><span data-stu-id="f3b80-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="f3b80-107">Seleccione la carpeta **Calendario**.</span><span class="sxs-lookup"><span data-stu-id="f3b80-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="f3b80-108">Vaya a la pestaña **Enviar**/**Recibir** y seleccione **Actualizar carpeta**.</span><span class="sxs-lookup"><span data-stu-id="f3b80-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="f3b80-109">Si aún no se actualiza el calendario o si faltan eventos, descargue la Herramienta de comprobación del calendario para Outlook desde el [centro de descarga de Microsoft](https://www.microsoft.com/download/details.aspx?id=28786).</span><span class="sxs-lookup"><span data-stu-id="f3b80-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="f3b80-110">Determine si hay más de 5 000 elementos en la carpeta de calendario, ya que esto puede causar síntomas como que no se actualicen las reuniones de calendario o errores de reunión.</span><span class="sxs-lookup"><span data-stu-id="f3b80-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="f3b80-111">Para más información, consulte [Problemas de rendimiento de Outlook cuando hay demasiados elementos o carpetas en un modo de almacenamiento en caché de archivos .ost o .pst](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span><span class="sxs-lookup"><span data-stu-id="f3b80-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>