---
title: Correo electrónico saliente a la carpeta correo no deseado
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096675"
---
# <a name="outbound-email-to-junk-email-folder"></a>Correo electrónico saliente a la carpeta correo no deseado

Si ve que los mensajes salientes se marcan como correo no deseado, siga estos pasos:

- Si aún no lo ha hecho, considere [la posibilidad de configurar las notificaciones de directivas de correo no deseado salientes](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Use [el seguimiento de](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) mensajes para ver si el mensaje saliente tiene el valor de evento **Correo** no deseado con el detalle adicional: Use grupo de entrega de **alto riesgo**.

  Para estos mensajes, compruebe el contenido del mensaje para ver lo que podría considerarse correo no deseado. Por ejemplo, las firmas a veces pueden causar problemas a muchos usuarios.

  Si tiene varios ejemplos de mensajes salientes legítimos que se marcan como correo no deseado, abra un vale de soporte técnico y pida al agente de soporte técnico que envíe sus mensajes como falsos positivos a nuestros analistas de correo no deseado. Esté preparado para proporcionar mensajes de ejemplo que incluyan todos los encabezados de mensaje.
