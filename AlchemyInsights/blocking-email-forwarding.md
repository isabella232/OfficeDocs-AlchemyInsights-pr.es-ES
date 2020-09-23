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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219872"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="c24be-102">Bloqueo o desbloqueo del reenvío de correo electrónico</span><span class="sxs-lookup"><span data-stu-id="c24be-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="c24be-103">Para habilitar o deshabilitar el reenvío de correo electrónico para un buzón específico, consulte [configurar el reenvío de correo electrónico](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="c24be-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="c24be-104">En el nivel de espacio empresarial, el control del reenvío externo se realiza con la Directiva de correo no deseado saliente.</span><span class="sxs-lookup"><span data-stu-id="c24be-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="c24be-105">Si se establece en OFF o Automatic, es posible que se bloquee el reenvío de correo con el error "550 5.7.520 acceso denegado, su organización no permite el reenvío externo".</span><span class="sxs-lookup"><span data-stu-id="c24be-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="c24be-106">A continuación, si el reenvío está configurado para bloquearse, es el error que verán los usuarios.</span><span class="sxs-lookup"><span data-stu-id="c24be-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="c24be-107">Si se está bloqueando el reenvío, asegúrese de que la Directiva está configurada para habilitar el autoenvío externo.</span><span class="sxs-lookup"><span data-stu-id="c24be-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="c24be-108">Puede comprobar la Directiva de filtro de correo no deseado saliente del centro de seguridad y cumplimiento o mediante la ejecución del comando Get-HostedOutboundSpamFilterPolicy | FL nombre, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="c24be-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="c24be-109">Si desea configurar el bloqueo de autoforward, el mismo comando le indicará el estado de la Directiva en este momento.</span><span class="sxs-lookup"><span data-stu-id="c24be-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="c24be-110">Nota: se recomienda mantener el autoenvío externo deshabilitado en la Directiva de filtro de correo no deseado saliente predeterminada y habilitarla solo para los usuarios que necesiten el reenvío externo mediante la creación de una directiva personalizada para esos usuarios.</span><span class="sxs-lookup"><span data-stu-id="c24be-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="c24be-111">Puede obtener más información en [configurar el reenvío externo de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="c24be-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>