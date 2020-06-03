---
title: Correo electrónico saliente a la carpeta correo electrónico no deseado
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511741"
---
# <a name="outbound-email-to-junk-email-folder"></a>Correo electrónico saliente a la carpeta correo electrónico no deseado

Si ve los mensajes salientes que se marcan como correo no deseado, siga estos pasos:

- Si todavía no lo ha hecho, considere la posibilidad de [configurar notificaciones de directivas de correo no deseado salientes](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Use el [seguimiento de mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) para ver si el mensaje saliente tiene el valor de evento **correo no deseado** con los detalles adicionales: **usar grupo de entrega de alto riesgo**.

  Para estos mensajes, compruebe el contenido del mensaje para ver lo que puede considerarse como correo no deseado. Por ejemplo, las firmas pueden causar problemas a muchos usuarios.

  Si tiene varios ejemplos de mensajes salientes legítimos que se marcan como correo no deseado, abra una incidencia de soporte técnico y solicite al agente de soporte técnico que envíe sus mensajes como falsos positivos a nuestros analistas de correo no deseado. Prepárese para proporcionar mensajes de ejemplo que incluyan todos los encabezados de mensajes.
