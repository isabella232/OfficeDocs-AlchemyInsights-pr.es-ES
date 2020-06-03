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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="2fc99-102">No se puede habilitar la auditoría unificada</span><span class="sxs-lookup"><span data-stu-id="2fc99-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="2fc99-103">Al intentar habilitar la auditoría unificada para su organización, es posible que reciba un error similar al siguiente:</span><span class="sxs-lookup"><span data-stu-id="2fc99-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="2fc99-104">Para resolver este problema, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="2fc99-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="2fc99-105">[Conéctese a Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="2fc99-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="2fc99-106">Ejecute el siguiente cmdlet:</span><span class="sxs-lookup"><span data-stu-id="2fc99-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="2fc99-107">Espere durante 60 minutos para que la configuración anterior surta efecto.</span><span class="sxs-lookup"><span data-stu-id="2fc99-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="2fc99-108">Ejecute el siguiente comando en Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2fc99-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="2fc99-109">Para obtener más información, vea los siguientes artículos:</span><span class="sxs-lookup"><span data-stu-id="2fc99-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="2fc99-110">Conectarse a PowerShell para Exchange Online con Multi-Factor Authentication</span><span class="sxs-lookup"><span data-stu-id="2fc99-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="2fc99-111">Activar o desactivar la búsqueda de registros de auditoría</span><span class="sxs-lookup"><span data-stu-id="2fc99-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
