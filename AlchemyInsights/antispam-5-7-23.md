---
title: Correo no deseado - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932186"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corregir problemas de entrega de correo electrónico para el código de error 5.7.23

Compruebe el registro DNS de SPF para su dominio en un SPF o un registrador de registros DNS disponibles públicamente en la web.

Compruebe que Microsoft no identificó el mensaje saliente como correo no deseado y que se enrutó a través del [grupo de entrega de alto riesgo](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Los mensajes del grupo de entrega de alto riesgo no pasarán comprobaciones de SPF y, por lo tanto, la organización de correo electrónico de destino no aceptará los mensajes.

Si el problema persiste, es posible que deba ponerse en contacto con el administrador del host de correo al que está intentando enviar correo electrónico. Anote el error externo detallado disponible en el mensaje de desbotón. Es posible que el soporte técnico de Microsoft no pueda ayudar más.
