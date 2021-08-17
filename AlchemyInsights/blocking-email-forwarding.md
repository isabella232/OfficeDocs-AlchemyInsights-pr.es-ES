---
title: 726 Bloqueo del reenvío de correo electrónico
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059649"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloqueo o desbloqueo del reenvío de correo electrónico

Para habilitar o deshabilitar el reenvío de correo electrónico para un buzón específico, vea [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

En el nivel de inquilino, el control del reenvío externo se realiza mediante la directiva de correo no deseado saliente. Puede comprobar la directiva de filtro de correo no deseado saliente desde el Centro de seguridad y cumplimiento [aquí](https://protection.office.com/antispam) o mediante el comando [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Si recibe el siguiente error: **"550 5.7.520 Acceso denegado,** Su organización no permite el reenvío externo", asegúrese de que la directiva está configurada para habilitar el reenvío automático externo.

**Nota:** Se recomienda mantener deshabilitada la opción Autoforward externo en la directiva de filtro de correo no deseado saliente predeterminada y habilitarla solo para los usuarios que necesiten reenvío externo mediante la creación de una directiva personalizada para esos usuarios. Puede leer más en [Configurar el reenvío de correo electrónico externo en Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).