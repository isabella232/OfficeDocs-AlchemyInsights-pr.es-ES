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
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloqueo o desbloqueo del reenvío de correo electrónico

Para habilitar o deshabilitar el reenvío de correo electrónico para un buzón específico, consulte [configurar el reenvío de correo electrónico](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

En el nivel de espacio empresarial, el control del reenvío externo se realiza mediante la Directiva de correo no deseado saliente. Puede consultar la Directiva de filtro de correo no deseado saliente desde el centro de seguridad y cumplimiento [aquí](https://protection.office.com/antispam) o mediante el [comando Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Si recibe el siguiente error: **"550 5.7.520 acceso denegado, su organización no permite el reenvío externo"**, asegúrese de que la Directiva está configurada para habilitar el reenvío automático externo.

**Nota:** Se recomienda mantener el autoenvío externo deshabilitado en la Directiva de filtro de correo no deseado saliente predeterminada y habilitarlo solo para los usuarios que necesiten el reenvío externo mediante la creación de una directiva personalizada para esos usuarios. Puede obtener más información en [configurar el reenvío externo de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).