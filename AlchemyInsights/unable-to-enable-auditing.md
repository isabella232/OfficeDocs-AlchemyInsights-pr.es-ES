---
title: 2419-no se puede-habilitar-auditoría
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510445"
---
# <a name="unable-to-enable-unified-auditing"></a>No se puede habilitar la auditoría unificada

Al intentar habilitar la auditoría unificada para su organización, es posible que reciba un error similar al siguiente:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Para resolver este problema, siga estos pasos:

1. [Conéctese a Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Ejecute el siguiente cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Espere durante 60 minutos para que la configuración anterior surta efecto.

4. Ejecute el siguiente comando en Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Para obtener más información, vea los siguientes artículos:

- [Conectarse a PowerShell para Exchange Online con Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activar o desactivar la búsqueda de registros de auditoría](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
