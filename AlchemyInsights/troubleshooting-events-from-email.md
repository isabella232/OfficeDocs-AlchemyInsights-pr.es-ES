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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105369"
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