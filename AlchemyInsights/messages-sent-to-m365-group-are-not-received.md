---
title: No todos los miembros reciben los mensajes que se envían al grupo de Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479470"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>No todos los miembros reciben los mensajes que se envían a un grupo de Microsoft 365

Asegúrese de que todos los miembros del grupo se hayan suscrito para recibir los correos. Consulte [Seguir a un grupo en Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Para comprobar el estado del mensaje de los miembros que se han suscrito a los correos electrónicos del grupo, ejecute el comando siguiente en [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Use el siguiente comando EXO PowerShell para establecer que todos los miembros del grupo reciban los correos enviados al grupo de Microsoft 365 en su bandeja de entrada:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Por ejemplo:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`