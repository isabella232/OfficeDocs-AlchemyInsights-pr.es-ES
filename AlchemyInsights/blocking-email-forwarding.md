---
title: 726 bloquear el reenvío de correo electrónico
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478323"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="5687e-102">Bloqueo o desbloqueo del reenvío de correo electrónico</span><span class="sxs-lookup"><span data-stu-id="5687e-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="5687e-103">Para habilitar o deshabilitar el reenvío de correo electrónico para un buzón específico, consulte [configurar el reenvío de correo electrónico](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5687e-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="5687e-104">En el nivel de espacio empresarial, el control del reenvío externo se realiza mediante la Directiva de correo no deseado saliente.</span><span class="sxs-lookup"><span data-stu-id="5687e-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="5687e-105">Puede consultar la Directiva de filtro de correo no deseado saliente desde el centro de seguridad y cumplimiento [aquí](https://protection.office.com/antispam) o mediante el [comando Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="5687e-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="5687e-106">Si recibe el siguiente error: **"550 5.7.520 acceso denegado, su organización no permite el reenvío externo"**, asegúrese de que la Directiva está configurada para habilitar el reenvío automático externo.</span><span class="sxs-lookup"><span data-stu-id="5687e-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="5687e-107">**Nota:** Se recomienda mantener el autoenvío externo deshabilitado en la Directiva de filtro de correo no deseado saliente predeterminada y habilitarlo solo para los usuarios que necesiten el reenvío externo mediante la creación de una directiva personalizada para esos usuarios.</span><span class="sxs-lookup"><span data-stu-id="5687e-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="5687e-108">Puede obtener más información en [configurar el reenvío externo de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5687e-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>