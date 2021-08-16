---
title: 'Para configurar la respuesta automática para todos los correos electrónicos enviados al grupo de Microsoft 365:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 3ed937d38627c1089c9203550498ce7b21ce01c0c5a2deea7326f8057f5338d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036149"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Para configurar la respuesta automática para todos los correos electrónicos enviados al grupo de Microsoft 365:

**Conecte a EXO PowerShell usando la cuenta de administrador del inquilino y use el siguiente comando**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> Cambie el **groupmailbox** a un nombre de grupo en el que desee configurar la respuesta automática como activada.

