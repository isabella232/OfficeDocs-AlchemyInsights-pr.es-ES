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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="f8024-102">Usar Exchange Online PowerShell para habilitar DKIM para un dominio específico</span><span class="sxs-lookup"><span data-stu-id="f8024-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="f8024-103">Si no puede crear los registros DNS DKIM en el Centro de administración, intente usar Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f8024-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="f8024-104">Para crear un registro DNS DKIM con Exchange Online PowerShell, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="f8024-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="f8024-105">Abra Windows PowerShell como administrador y ejecute los siguientes comandos en la secuencia descrita:</span><span class="sxs-lookup"><span data-stu-id="f8024-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="f8024-106">a.</span><span class="sxs-lookup"><span data-stu-id="f8024-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="f8024-107">b.</span><span class="sxs-lookup"><span data-stu-id="f8024-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="f8024-108">c.</span><span class="sxs-lookup"><span data-stu-id="f8024-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="f8024-109">Si tiene problemas para conectarse a Exchange Online PowerShell, vea [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="f8024-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="f8024-110">Una vez que esté conectado a Exchange Online PowerShell, ejecute el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="f8024-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="f8024-111">Una vez ejecutado correctamente el comando anterior, ejecute el siguiente comando para finalizar la sesión de PowerShell de Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="f8024-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



