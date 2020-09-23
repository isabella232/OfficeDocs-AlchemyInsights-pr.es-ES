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
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloqueo o desbloqueo del reenvío de correo electrónico

Para habilitar o deshabilitar el reenvío de correo electrónico para un buzón específico, consulte [configurar el reenvío de correo electrónico](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

En el nivel de espacio empresarial, el control del reenvío externo se realiza con la Directiva de correo no deseado saliente. Si se establece en OFF o Automatic, es posible que se bloquee el reenvío de correo con el error "550 5.7.520 acceso denegado, su organización no permite el reenvío externo". A continuación, si el reenvío está configurado para bloquearse, es el error que verán los usuarios.

Si se está bloqueando el reenvío, asegúrese de que la Directiva está configurada para habilitar el autoenvío externo. Puede comprobar la Directiva de filtro de correo no deseado saliente del centro de seguridad y cumplimiento o mediante la ejecución del comando Get-HostedOutboundSpamFilterPolicy | FL nombre, AutoForwardingMode. Si desea configurar el bloqueo de autoforward, el mismo comando le indicará el estado de la Directiva en este momento.

Nota: se recomienda mantener el autoenvío externo deshabilitado en la Directiva de filtro de correo no deseado saliente predeterminada y habilitarla solo para los usuarios que necesiten el reenvío externo mediante la creación de una directiva personalizada para esos usuarios. Puede obtener más información en [configurar el reenvío externo de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).