---
title: Error al enviar correo electrónico bloqueado por SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813741"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Error al enviar correo electrónico: host de cliente bloqueado con Spamhaus

La dirección IP que envió el mensaje se encuentra en una lista de bloqueo propiedad de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Entre los motivos de bloqueo de Spamhaus se incluyen cuentas comprometidas, máquinas comprometidas que comparten una dirección IP pública y directivas de proveedor de servicios de Internet (ISP). Las correcciones posibles son:
  
- Para los mensajes entrantes bloqueados donde controla el servidor de correo electrónico de origen, debe determinar la causa y quitar el bloque del sitio web de Spamhaus.

- Para los mensajes entrantes bloqueados en los que la dirección IP de origen pertenece a otra persona, el propietario de la dirección debe quitar el bloque del sitio web de Spamhaus. Si la dirección IP está en la lista de directivas bloqueados (PBL), el propietario puede asignar una dirección IP estática diferente o quitar la dirección del PBL.

- Para los mensajes salientes bloqueados de su dominio conectado a Microsoft, puede recibir este error si los mensajes se enruta a través de un servicio de terceros. Puede usar una herramienta de búsqueda WHOIS para buscar el propietario de la dirección IP bloqueada.
