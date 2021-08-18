---
title: Bloquear o desbloquear el reenvío automático de correo electrónico externo
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315891"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Bloquear o desbloquear el reenvío automático de correo electrónico eterno

Para habilitar o deshabilitar el reenvío de correo electrónico para un buzón específico, vea [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Los administradores pueden controlar el reenvío externo para la organización mediante [directivas de correo no deseado salientes.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Las directivas de correo no deseado salientes se administran en el portal de Microsoft 365 Defender o mediante el <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) en Exchange Online PowerShell.

Si recibe el siguiente error: **"550 5.7.520 Acceso denegado,** Su organización no permite el reenvío externo", asegúrese de que la directiva está configurada para habilitar los mensajes de reenvío automático externos.

**Nota:** Se recomienda el valor predeterminado  **Automático:** sistema controlado para la configuración de reglas de reenvío automático en la directiva de filtro de correo no deseado saliente predeterminada (el reenvío externo automático está bloqueado; el reenvío automático interno sigue funcionando). Debe crear directivas de filtro de correo no deseado saliente personalizadas y usar el valor **Activado: el** reenvío solo está habilitado para los usuarios que necesiten reenvío automático de correo electrónico externo. Para obtener más información, vea [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
