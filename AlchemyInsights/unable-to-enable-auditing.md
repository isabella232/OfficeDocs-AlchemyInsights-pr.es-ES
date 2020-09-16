---
title: 2419-no se puede-habilitar-auditoría
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767616"
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
