---
title: Se ha recibido el NDR completo AggregateGroupMailbox para el correo electrónico enviado al grupo de Microsoft 365
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
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715725"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Se ha recibido el NDR completo AggregateGroupMailbox para el correo electrónico enviado al grupo de Microsoft 365

Use el siguiente comando de Shell EXO para crear una regla de transporte de Exchange para eliminar los correos electrónicos enviados al buzón de grupo agregado de forma silenciosa:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Reemplace la dirección SMTP en **-sentto** con la dirección SMTP del grupo de buzones de grupo agregado en su espacio empresarial. Puede obtener la dirección SMTP del buzón de grupo agregado del NDR recibido.



