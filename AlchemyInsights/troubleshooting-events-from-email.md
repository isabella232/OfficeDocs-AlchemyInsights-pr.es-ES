---
title: Solución de problemas de eventos desde el correo electrónico
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658751"
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