---
title: Correo electrónico saliente a la carpeta correo electrónico no deseado
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
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769200"
---
# <a name="outbound-email-to-junk-email-folder"></a>Correo electrónico saliente a la carpeta correo electrónico no deseado

Si ve los mensajes salientes que se marcan como correo no deseado, siga estos pasos:

- Si todavía no lo ha hecho, considere la posibilidad de [configurar notificaciones de directivas de correo no deseado salientes](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Use el [seguimiento de mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) para ver si el mensaje saliente tiene el valor de evento **correo no deseado** con los detalles adicionales: **usar grupo de entrega de alto riesgo**.

  Para estos mensajes, compruebe el contenido del mensaje para ver lo que puede considerarse como correo no deseado. Por ejemplo, las firmas pueden causar problemas a muchos usuarios.

  Si tiene varios ejemplos de mensajes salientes legítimos que se marcan como correo no deseado, abra una incidencia de soporte técnico y solicite al agente de soporte técnico que envíe sus mensajes como falsos positivos a nuestros analistas de correo no deseado. Prepárese para proporcionar mensajes de ejemplo que incluyan todos los encabezados de mensajes.
