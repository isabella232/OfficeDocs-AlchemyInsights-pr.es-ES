---
title: Usar Exchange Online PowerShell para habilitar DKIM para un dominio específico
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737655"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Usar Exchange Online PowerShell para habilitar DKIM para un dominio específico

Si no puede crear los registros DNS DKIM en el Centro de administración, intente usar Exchange Online PowerShell. 

Para crear un registro DNS DKIM con Exchange Online PowerShell, siga estos pasos:

1. Abra Windows PowerShell como administrador y ejecute los siguientes comandos en la secuencia descrita:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Si tiene problemas para conectarse a Exchange Online PowerShell, vea [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Una vez que esté conectado a Exchange Online PowerShell, ejecute el siguiente comando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Una vez ejecutado correctamente el comando anterior, ejecute el siguiente comando para finalizar la sesión de PowerShell de Exchange Online:

    `Remove-PSSession $Session` 



