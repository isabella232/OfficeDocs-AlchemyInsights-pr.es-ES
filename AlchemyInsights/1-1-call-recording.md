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
# <a name="11-call-recording"></a>Grabación de llamadas 1:1

Los administradores deben tomar medidas ahora para seguir permitiendo a los usuarios registrar llamadas 1:1.
 
A partir del 12 de abril de 2021, empezaremos a aplicar una nueva opción de directiva de llamadas de Teams *AllowCloudRecordingForCalls*. 

Actualmente, las capacidades de grabación de llamadas 1:1 están controladas por *la opción AllowCloudRecording* en Directivas de reunión de Teams. Si los usuarios pueden grabar reuniones de Teams, también pueden registrar llamadas 1:1.

Si prefiere impedir que todos los usuarios graben llamadas 1:1, no es necesario realizar ninguna acción. La opción de directiva de llamada *AllowCloudRecordingForCalls* se $False de forma predeterminada.

Este cambio se documenta en la siguiente publicación del Centro de mensajes: [(actualizada) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Introducción a la directiva de registro de llamadas Para establecer la opción directiva de llamadas de Teams, debe usar [PowerShell de Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Para habilitar la grabación de llamadas en llamadas 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

Para deshabilitar la grabación de llamadas en llamadas **1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

