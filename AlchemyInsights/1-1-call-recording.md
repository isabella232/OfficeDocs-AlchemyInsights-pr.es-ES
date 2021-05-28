---
title: Grabación de llamadas 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696975"
---
# <a name="11-call-recording"></a><span data-ttu-id="e2167-102">Grabación de llamadas 1:1</span><span class="sxs-lookup"><span data-stu-id="e2167-102">1:1 call recording</span></span>

<span data-ttu-id="e2167-103">Si el **botón Iniciar grabación** está atenuado en una llamada 1:1, debe cambiar la configuración de directiva para el usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="e2167-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="e2167-104">A partir del 31 de mayo de 2021, empezaremos a aplicar una nueva directiva de Teams de llamadas *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="e2167-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="e2167-105">Antes de este cambio, la grabación de llamadas 1:1 está controlada por la Directiva de reuniones *allowCloudRecording* Teams de reuniones.</span><span class="sxs-lookup"><span data-stu-id="e2167-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="e2167-106">Este cambio se documenta en la entrada del Centro de mensajes: [(Actualizado) 1:1 Introducción](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)a la directiva de registro de llamadas .</span><span class="sxs-lookup"><span data-stu-id="e2167-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="e2167-107">*AllowCloudRecordingForCalls*   la opción de directiva de llamada **se establece $False** de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="e2167-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="e2167-108">Si prefieres impedir que todos los usuarios graben llamadas 1:1, no necesitas realizar ninguna acción.</span><span class="sxs-lookup"><span data-stu-id="e2167-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="e2167-109">Para habilitar el registro de llamadas para todos los usuarios en llamadas 1:1, use Teams PowerShell para ejecutar el siguiente cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e2167-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="e2167-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="e2167-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="e2167-111">Como alternativa, puedes crear una nueva directiva y establecer **-AllowCloudRecordingForCalls** para $true y asignar esa directiva a los usuarios. </span><span class="sxs-lookup"><span data-stu-id="e2167-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="e2167-112">Para obtener más información, [vea 1:1 Call Recording Policy Controls Are (Almost!) Aquí](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="e2167-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
