---
title: Administrar registro en diario
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737491"
---
# <a name="manage-journaling"></a><span data-ttu-id="80392-102">Administrar registro en diario</span><span class="sxs-lookup"><span data-stu-id="80392-102">Manage journaling</span></span>

<span data-ttu-id="80392-103">El registro en diario puede ayudar a la organización a responder a los requisitos de cumplimiento legal, normativo y organizativo mediante el registro de las comunicaciones de correo electrónico entrantes y salientes.</span><span class="sxs-lookup"><span data-stu-id="80392-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="80392-104">Recuerde:</span><span class="sxs-lookup"><span data-stu-id="80392-104">Keep in mind:</span></span>

* <span data-ttu-id="80392-105">Debe tener permisos de [administración de la organización](https://go.microsoft.com/fwlink/?linkid=2115259) y administración [de](https://go.microsoft.com/fwlink/?linkid=2115469) registros para poder administrar el registro en diario.</span><span class="sxs-lookup"><span data-stu-id="80392-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="80392-106">Debe tener configurado un buzón de diario y (opcionalmente) un buzón de registro en diario alternativo.</span><span class="sxs-lookup"><span data-stu-id="80392-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="80392-107">Para obtener más información, vea [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="80392-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="80392-108">En Exchange Online, hay un límite en el número de reglas de diario que puede crear.</span><span class="sxs-lookup"><span data-stu-id="80392-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="80392-109">Para obtener más información, vea Límites de [reglas de diario, transporte y bandeja de entrada.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="80392-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="80392-p104">Exchange Online no admite la entrega de informes de diario a un buzón de correo de Exchange Online. Debe especificar la dirección de correo electrónico de un sistema de archivado local o un servicio de archivado de terceros como buzón de correo de registro en diario.</span><span class="sxs-lookup"><span data-stu-id="80392-p104">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox. You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
