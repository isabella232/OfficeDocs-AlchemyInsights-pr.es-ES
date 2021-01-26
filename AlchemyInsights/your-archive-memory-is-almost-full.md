---
title: El buzón de archivo está casi lleno
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950516"
---
# <a name="your-archive-mailbox-is-almost-full"></a>El buzón de archivo está casi lleno

Si el usuario recibe la advertencia; **El buzón de archivo está casi** lleno, o necesita aumentar el tamaño de su buzón de archivo, estas son algunas sugerencias:

1. Si al usuario se le asigna un Plan 1 de Exchange Online, actualice a la licencia del **Plan 2** de Exchange Online para aumentar el tamaño de 50 GB a 100 GB.
1. Si el usuario ya tiene asignada una de las siguientes opciones: **Exchange Online Plan 2** o Exchange Online Plan 1 con un complemento Archivado de Exchange Online, siga estos pasos para habilitar el archivado de expansión automática:.
 
    1. [Conéctese a Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Ejecute el siguiente commandlet para el usuario:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Ejecute el siguiente commandlet para confirmar que está habilitado para el usuario:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Para obtener más información, vea:

- [ Habilitar el archivado ilimitado- Ayuda para administradores- Cumplimiento de Microsoft 365 | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Límites de Exchange Online: descripción del servicio | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Actualizar a un plan de negocio | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

