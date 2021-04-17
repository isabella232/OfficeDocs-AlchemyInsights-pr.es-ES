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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821428"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corregir problemas de entrega de correo electrónico para el código de error 5.7.23

Compruebe el registro DNS de SPF para su dominio en un SPF o un registrador de registros DNS disponibles públicamente en la web.

Compruebe que Microsoft no identificó el mensaje saliente como correo no deseado y que se enrutó a través del [grupo de entrega de alto riesgo](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Los mensajes del grupo de entrega de alto riesgo no pasarán comprobaciones de SPF y, por lo tanto, la organización de correo electrónico de destino no aceptará los mensajes.

Si el problema persiste, es posible que deba ponerse en contacto con el administrador del host de correo al que está intentando enviar correo electrónico. Anote el error externo detallado disponible en el mensaje de desbotón. Es posible que el soporte técnico de Microsoft no pueda ayudar más.
