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
ms.openlocfilehash: 28267a4cd0aa139467327385b8e85fed1675cf19
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533004"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Prueba de la configuración de IRM para nuevas funcionalidades de OME

Para comprobar que el espacio empresarial de Microsoft 365 está configurado para usar nuevas funcionalidades de OME, ejecute los siguientes cmdlets mientras está conectado al [PowerShell de Exchange Online](/powershell/exchange/exchange-online-powershell):


1. Compruebe la configuración de IRM del espacio empresarial ejecutando `Get-IRMConfiguration`. Asegúrese de que estos valores están establecidos en **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Con el dominio, la dirección del remitente y el destinatario, ejecute `Test-IRMConfiguration`. Si la prueba no se supera, investigue la configuración de IRM.

Para más información sobre cómo comprobar la configuración de IRM, vea [Comprobar la nueva configuración de OME en PowerShell de Exchange Online](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).