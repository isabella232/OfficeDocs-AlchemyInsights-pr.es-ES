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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="f78a2-102">El remitente no recibe el correo electrónico enviado al grupo de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f78a2-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="f78a2-103">De forma predeterminada, el remitente de un mensaje de correo electrónico a un grupo de Microsoft 365 no recibe una copia del mensaje en la bandeja de entrada, aunque es un miembro del grupo.</span><span class="sxs-lookup"><span data-stu-id="f78a2-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="f78a2-104">Use este comando PowerShell EXO para permitir que el remitente reciba una copia de todos los mensajes de correo electrónico que envíen al grupo de Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="f78a2-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="f78a2-105">Para habilitar la configuración para todos los buzones a la vez, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f78a2-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="f78a2-106">**Nota** Los cambios de esta configuración tardan hasta una hora en surtir efecto.</span><span class="sxs-lookup"><span data-stu-id="f78a2-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>