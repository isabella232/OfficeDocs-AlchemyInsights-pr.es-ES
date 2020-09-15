---
title: Contra correo electrónico no deseado-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717342"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corregir problemas de entrega de correo electrónico para el código de error 5.7.23

Compruebe el registro DNS de SPF de su dominio en un SPF o un comprobador de registros DNS disponible públicamente en la Web.

Compruebe que Microsoft no identificó el mensaje saliente como correo no deseado y se enrutó a través del [grupo de entrega de alto riesgo](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Los mensajes del grupo de entrega de alto riesgo no pasarán las comprobaciones de SPF y, por lo tanto, no serán aceptados por la organización de correo electrónico de destino.

Si el problema persiste, es posible que deba ponerse en contacto con el administrador del host de correo al que está intentando enviar correo electrónico. Tome nota del error externo detallado disponible en el mensaje de devolución. Es posible que el soporte técnico de Microsoft no pueda ayudarle más.
