---
title: Aplicación del límite de recepción de buzones
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829172"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Aplicación del límite de recepción de buzones

Microsoft inició recientemente la aplicación del umbral por buzón de correo de 3600 mensajes por hora. Para más información, vea [Límites de Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Los buzones de correo de Microsoft 365 que reciben más de 3600 mensajes en una hora se limitan durante los próximos 60 minutos. 

Además, se aplica el límite de pares remitente-destinatario (SRP) que bloquea los mensajes recibidos por un buzón Microsoft 365 de un remitente específico. Si un solo remitente envía más del 33 % del umbral total o 1200 mensajes por hora continua a un destinatario específico, el límite de SRP se inicia y el buzón ya no acepta mensajes de ese remitente. Tenga en cuenta lo siguiente:

- Este límite se aplica a los correos electrónicos recibidos de otros espacios empresariales, remitentes locales o de Internet.
- La entrega de correo electrónico al buzón se bloquea durante los próximos 60 minutos. 
- Los remitentes a estos buzones reciben un informe de no entrega (5.2.121 o 5.2.122) que indica que el buzón ha superado el umbral máximo de entrega. El correo interno (correo dentro del mismo espacio empresarial) continúa en entrega.
- Cuando se aplica el límite SRP, el buzón de recepción sigue aceptando mensajes de otros remitentes.

Los administradores pueden supervisar la actividad actual del buzón de correo mediante el acceso a un nuevo informe e información en el centro de administración de Exchange denominado "Buzones que superan los límites de recepción". La información solo aparece si un espacio empresarial tiene buzones ofensivos, mientras que el informe siempre aparece en el panel, pero estará vacío a menos que un espacio empresarial tenga buzones ofensivos.

Para obtener más información sobre los límites de recepción de información, vea [Información sobre los buzones que superan los límites de recepción en el nuevo EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Para obtener más información sobre el informe acerca de la superación de los límites de recepción, vea [Informe sobre los buzones que superan los límites de recepción en el nuevo EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).