---
title: El remitente no recibe el correo electrónico enviado al grupo de Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751332"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>El remitente no recibe el correo electrónico enviado al grupo de Microsoft 365

De forma predeterminada, el remitente de un mensaje de correo electrónico a un grupo de Microsoft 365 no recibe una copia del mensaje en la bandeja de entrada, aunque es un miembro del grupo.

Use este comando PowerShell EXO para permitir que el remitente reciba una copia de todos los mensajes de correo electrónico que envíen al grupo de Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Para habilitar la configuración para todos los buzones a la vez, haga lo siguiente:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Nota** Los cambios de esta configuración tardan hasta una hora en surtir efecto.