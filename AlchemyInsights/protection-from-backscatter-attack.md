---
title: Protección contra un ataque de devolución de correo no enviado
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898024"
---
# <a name="protection-from-backscatter-attack"></a>Protección contra un ataque de devolución de correo no enviado

La devolución de correo no enviado son informes no entregados (también conocidos como NDR o mensajes de devolución) que recibe de mensajes que no envió. Los emisores de correo electrónico no deseado falsifican (suplantan electrónicamente) la dirección **De:** de sus mensajes y, a menudo, utilizan direcciones de correo electrónico reales para dar credibilidad a sus mensajes. Entonces, cuando los emisores de correo electrónico no deseado envían mensajes a destinatarios inexistentes de forma inevitable, el servidor de correo electrónico de destino es esencialmente engañado para que devuelva el mensaje no entregado en un informe de no entrega al remitente falsificado en la dirección **De:**.

Puede encontrar información adicional en [Devolución de correo no enviado en EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Habilitar la protección contra la devolución de correo no enviado**

Para habilitar la protección contra la devolución de correo no enviado, siga la ruta a continuación.

**protection.office.com > Administración de amenazas > Directiva > Antispam > Seleccione la Directiva de filtro contra correo no deseado > Propiedades de correo no deseado > Marque como correo no deseado > devolución de correo no enviado NDR > Asignar como «activado»**

Si cree que una cuenta se ha visto comprometida, consulte lo siguiente:

- [Responder a una cuenta de correo electrónico en peligro](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Quitar usuarios bloqueados del portal de usuarios restringidos en Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



