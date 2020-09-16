---
title: Mensaje de bienvenida en grupos de Microsoft 365
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
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725856"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Mensaje de bienvenida en grupos de Microsoft 365

Los nuevos usuarios que se unan al grupo de Microsoft 365 recibirán un correo electrónico de bienvenida si la propiedad "UnifiedGroupWelcomeMessageEnabled" está establecida en True.

Si desea deshabilitar el mensaje de bienvenida, use el siguiente comando de [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps):

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
