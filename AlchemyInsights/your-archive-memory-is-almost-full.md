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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046769"
---
# <a name="your-archive-mailbox-is-almost-full"></a>El buzón de archivo está casi lleno

Si el usuario recibe la advertencia; **El buzón de archivo está casi** lleno, o necesita aumentar el tamaño de su buzón de archivo, a continuación se de algunas sugerencias:

1. Si al usuario se le asigna un Exchange Online plan 1, actualice Exchange Online una licencia del **Plan 2** para aumentar el tamaño de 50 GB a 100 GB.
1. Si el usuario ya tiene asignado uno de los siguientes procedimientos: **Exchange Online Plan 2** o un plan 1 de Exchange Online con un complemento Archivado de Exchange Online, siga estos pasos para habilitar el archivado de expansión automática:.
 
    1. [Conectar a Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Ejecute el siguiente commandlet para el usuario:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Ejecute el siguiente commandlet para confirmar que está habilitado para el usuario:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Para más información, consulte:

- [Habilitar el archivado ilimitado: Ayuda para administradores: Microsoft 365 cumplimiento | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online límites: descripciones de servicio | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Actualizar a un plan de negocio | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

