---
title: Solución de problemas de eventos desde el correo electrónico
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834856"
---
# <a name="troubleshooting-events-from-email"></a>Solución de problemas de eventos desde el correo electrónico

1. Compruebe que la característica está habilitada para el buzón: **Get-EventsFromEmailConfiguration-Identity <mailbox>**

2. Después, consulte los registros de "Eventos desde el correo electrónico" **Export-MailboxDiagnosticLogs <mailbox>-Component TimeProfile**

3. En los registros de "Eventos desde el correo electrónico", busque el InternetMessageId que coincida con el elemento en el buzón.  

4. TrustScore determina si el elemento está o no agregado. Solo se agregarán eventos si TrustScore = "De confianza".

TrustScore está determinada por las propiedades SPF, Dkim o Dmarc que aparecen en el encabezado del mensaje.

Para ver estas propiedades:

**Escritorio de Outlook**

- Abrir el elemento
- Archivo -> Propiedades -> Encabezados de Internet

o

**MFCMapi**

- Ir al elemento en la bandeja de entrada
- Buscar PR_TRANSPORT_MESSAGE_HEADERS_W

Estas propiedades se determinan y se registran durante el transporte y enrutamiento. Para solucionar problemas adicionales, es posible que tenga que realizar un seguimiento con el Soporte de transporte sobre los errores en SPF, DKIM y DMARC.