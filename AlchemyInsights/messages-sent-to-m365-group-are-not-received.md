---
title: No todos los miembros reciben los mensajes que se envían al grupo de Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806164"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>No todos los miembros reciben los mensajes que se envían a un grupo de Microsoft 365

Asegúrese de que todos los miembros del grupo se hayan suscrito para recibir los correos. Consulte [Seguir a un grupo en Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Para comprobar el estado del mensaje de los miembros que se han suscrito a los correos electrónicos del grupo, ejecute el comando siguiente en [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`