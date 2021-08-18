---
title: ¿Necesita ayuda con los límites de envío de correo electrónico?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: a13eec5d0d1abccd748653e7d7d9bb999b2e3b7a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58328843"
---
# <a name="need-help-with-email-sending-limits"></a>¿Necesita ayuda con los límites de envío de correo electrónico?

A continuación se muestran los **límites de envío por diseño** aplicados en el servicio. Más información sobre estos límites [aquí](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- Para desalentar la entrega de mensajes masivos no solicitados, aplicamos **límites de tasa de destinatario por usuario a todos los mensajes salientes e internos**. En todas las SKU, este límite es de **10 000 destinatarios por día**.  Los clientes que deban enviar un correo electrónico comercial masivo válido (por ejemplo, boletines para clientes) deberían usar proveedores de terceros especializados en dichos servicios.
    **Nota**: una vez que se alcanza el límite de tasa de destinatarios, no se pueden enviar mensajes desde el buzón de correo hasta que la cantidad de destinatarios a los que se enviaron mensajes en las últimas 24 horas baje por debajo del límite. El usuario no podrá enviar mensajes hasta ese momento.
- Se aplica un límite de tasa de mensajes de **30 mensajes por minuto** en todas las SKU. Esto determina cuántos mensajes puede enviar un usuario desde la cuenta de Exchange online en un período de tiempo especificado.
- El **número máximo de destinatarios permitido en los campos Para, CC y CCO** en un solo mensaje de correo electrónico en todas las SKU, es de **1000 destinatarios**. Si desea personalizar el límite, consulte [este vínculo](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
