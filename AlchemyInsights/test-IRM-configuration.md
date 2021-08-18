---
title: Prueba de la configuración de IRM para nuevas funcionalidades de OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899713"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Prueba de la configuración de IRM para nuevas funcionalidades de OME

Para comprobar que el espacio empresarial de Microsoft 365 está configurado para usar nuevas funcionalidades de OME, ejecute los siguientes cmdlets mientras está conectado al [PowerShell de Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell):


1. Compruebe la configuración de IRM del espacio empresarial ejecutando `Get-IRMConfiguration`. Asegúrese de que estos valores están establecidos en **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Con el dominio, la dirección del remitente y el destinatario, ejecute `Test-IRMConfiguration`. Si la prueba no se supera, investigue la configuración de IRM.

Para más información sobre cómo comprobar la configuración de IRM, vea [Comprobar la nueva configuración de OME en PowerShell de Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).