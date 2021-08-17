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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314401"
---
# <a name="11-call-recording"></a>Grabación de llamadas 1:1

Si el **botón Iniciar grabación** está atenuado en una llamada 1:1, debe cambiar la configuración de directiva para el usuario afectado. Para comprobar la configuración de directiva, ejecute el diagnóstico para el usuario afectado escribiendo Diag: Teams registro de llamadas **1:1** anterior.     

A partir del 31 de mayo de 2021, empezaremos a aplicar una nueva directiva de Teams de llamadas *AllowCloudRecordingForCalls*. Antes de este cambio, la grabación de llamadas 1:1 está controlada por la Directiva de reuniones *allowCloudRecording* Teams de reuniones. Este cambio se documenta en la entrada del Centro de mensajes: [(Actualizado) 1:1 Introducción](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)a la directiva de registro de llamadas .  

*AllowCloudRecordingForCalls*   la opción de directiva de llamada **se establece $False** de forma predeterminada. Si prefieres impedir que todos los usuarios graben llamadas 1:1, no necesitas realizar ninguna acción.  

Para habilitar la grabación de llamadas para todos los usuarios en llamadas 1:1, [use Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) para ejecutar el siguiente cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Como alternativa, puedes crear una nueva directiva y establecer **-AllowCloudRecordingForCalls** para $true y asignar esa directiva a los usuarios.  

Para obtener más información, [vea 1:1 Call Recording Policy Controls Are (Almost!) Aquí](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
