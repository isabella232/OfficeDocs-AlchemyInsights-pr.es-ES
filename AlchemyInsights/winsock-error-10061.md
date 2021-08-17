---
title: Error 1554 Winsock 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083247"
---
# <a name="winsock-error-10061"></a>Error winsock 10061

Este código de error significa que Microsoft no pudo establecer un socket TCP (conexión) con el host de destino. La causa más probable de este error es un problema con la configuración del firewall. Para solucionar el problema, compruebe esta configuración:

- Compruebe la configuración del firewall con la información Microsoft 365 direcciones URL e [intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Si el error es específico de Exchange Online Protection (EOP), se le debería haber notificado previamente un cambio en las direcciones [IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)de Exchange Online Protection .

- Compruebe que el proveedor de servicios de Internet (ISP) no está bloqueando el puerto.

- Compruebe la configuración del host inteligente y del servidor de destino en los conectores.

Tenga en cuenta Microsoft 365 no bloquea las *conexiones* entrantes de esta manera.
