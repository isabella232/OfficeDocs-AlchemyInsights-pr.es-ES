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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733866"
---
# <a name="11-call-recording"></a><span data-ttu-id="05651-102">Grabación de llamadas 1:1</span><span class="sxs-lookup"><span data-stu-id="05651-102">1:1 call recording</span></span>

<span data-ttu-id="05651-103">Los administradores deben tomar medidas ahora para seguir permitiendo a los usuarios registrar llamadas 1:1.</span><span class="sxs-lookup"><span data-stu-id="05651-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="05651-104">A partir del 12 de abril de 2021, empezaremos a aplicar una nueva opción de directiva de llamadas de Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="05651-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="05651-105">Actualmente, las capacidades de grabación de llamadas 1:1 están controladas por *la opción AllowCloudRecording* en Directivas de reunión de Teams.</span><span class="sxs-lookup"><span data-stu-id="05651-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="05651-106">Si los usuarios pueden grabar reuniones de Teams, también pueden registrar llamadas 1:1.</span><span class="sxs-lookup"><span data-stu-id="05651-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="05651-107">Si prefiere impedir que todos los usuarios graben llamadas 1:1, no es necesario realizar ninguna acción.</span><span class="sxs-lookup"><span data-stu-id="05651-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="05651-108">La opción de directiva de llamada *AllowCloudRecordingForCalls* se $False de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="05651-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="05651-109">Este cambio se documenta en la siguiente publicación del Centro de mensajes: [(actualizada) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Introducción a la directiva de registro de llamadas Para establecer la opción directiva de llamadas de Teams, debe usar [PowerShell de Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="05651-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="05651-110">**Para habilitar la grabación de llamadas en llamadas 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="05651-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="05651-111">Para deshabilitar la grabación de llamadas en llamadas **1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="05651-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

