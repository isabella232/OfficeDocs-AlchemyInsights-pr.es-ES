---
title: Enviar como grupo de Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740168"
---
# <a name="send-as-microsoft-365-group"></a>Enviar como grupo de Microsoft 365

Puede asignar permisos de Enviar como, para permitir que usuarios específicos envíen mensajes como un grupo de Microsoft 365:  

1. Conexión a Exchange Online PowerShell.  

2. Ejecute el siguiente comando:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Para obtener más información, consulte [Permitir que los miembros envíen como o envíen en nombre de un grupo](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).