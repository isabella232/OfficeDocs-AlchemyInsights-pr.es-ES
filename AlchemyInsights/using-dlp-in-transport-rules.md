---
title: Usar DLP en reglas de transporte
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
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084111"
---
# <a name="using-dlp-in-transport-rules"></a>Usar DLP en reglas de transporte

Para integrar la Prevención de pérdida de datos (DLP) en un transporte existente, use la condición "**Si el mensaje contiene... Información confidencial**"en la configuración de la regla de transporte.

**Para información más detallada, consulte:**

- Tipos de información confidencial de DLP integrados en las reglas de transporte: [Integrar reglas de información confidencial](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

También puede probar la regla con o sin prueba de directiva con el Modo de prueba en la regla.  Debería esperar 30 minutos después de crear la regla antes de probarla.

- Consulte [Probar el flujo de correo o las reglas de transporte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Nota**: si está intentando implementar una directiva DLP nueva con las reglas de transporte en el Centro de administración de Exchange, use [directivas DLP en el Centro de seguridad y cumplimiento](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) en su lugar.
