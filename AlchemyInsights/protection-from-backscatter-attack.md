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
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="45a79-102">Protección contra un ataque de devolución de correo no enviado</span><span class="sxs-lookup"><span data-stu-id="45a79-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="45a79-103">La devolución de correo no enviado son informes no entregados (también conocidos como NDR o mensajes de devolución) que recibe de mensajes que no envió.</span><span class="sxs-lookup"><span data-stu-id="45a79-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="45a79-104">Los emisores de correo electrónico no deseado falsifican (suplantan electrónicamente) la dirección **De:** de sus mensajes y, a menudo, utilizan direcciones de correo electrónico reales para dar credibilidad a sus mensajes.</span><span class="sxs-lookup"><span data-stu-id="45a79-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="45a79-105">Entonces, cuando los emisores de correo electrónico no deseado envían mensajes a destinatarios inexistentes de forma inevitable, el servidor de correo electrónico de destino es esencialmente engañado para que devuelva el mensaje no entregado en un informe de no entrega al remitente falsificado en la dirección **De:**.</span><span class="sxs-lookup"><span data-stu-id="45a79-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="45a79-106">Puede encontrar información adicional en [Devolución de correo no enviado en EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="45a79-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="45a79-107">**Habilitar la protección contra la devolución de correo no enviado**</span><span class="sxs-lookup"><span data-stu-id="45a79-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="45a79-108">Para habilitar la protección contra la devolución de correo no enviado, siga la ruta a continuación.</span><span class="sxs-lookup"><span data-stu-id="45a79-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="45a79-109">**protection.office.com > Administración de amenazas > Directiva > Antispam > Seleccione la Directiva de filtro contra correo no deseado > Propiedades de correo no deseado > Marque como correo no deseado > devolución de correo no enviado NDR > Asignar como «activado»**</span><span class="sxs-lookup"><span data-stu-id="45a79-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="45a79-110">Si cree que una cuenta se ha visto comprometida, consulte lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="45a79-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="45a79-111">Responder a una cuenta de correo electrónico en peligro</span><span class="sxs-lookup"><span data-stu-id="45a79-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="45a79-112">Quitar usuarios bloqueados del portal de usuarios restringidos en Office 365</span><span class="sxs-lookup"><span data-stu-id="45a79-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



