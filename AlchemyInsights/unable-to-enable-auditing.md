---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007807"
---
# <a name="unable-to-enable-unified-auditing"></a>No se puede habilitar la auditoría unificada

Cuando intenta habilitar la auditoría unificada para su organización, puede recibir un error similar al siguiente:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Para resolver este problema, siga estos pasos:

1. [Conectar a Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Ejecute el siguiente cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Espere 60 minutos para que la configuración anterior suba a efecto.

4. Ejecute el siguiente comando en Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Para obtener información adicional, consulte los artículos siguientes:

- [Conectarse a PowerShell para Exchange Online con Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activar o desactivar la búsqueda de registros de auditoría](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
