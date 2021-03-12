---
title: Establecer ClientAccessServerEnabled en True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737692"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="bf24d-102">Establecer ClientAccessServerEnabled en True</span><span class="sxs-lookup"><span data-stu-id="bf24d-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="bf24d-103">Si no puede abrir un mensaje de correo electrónico cifrado y, en su lugar, ver los datos **adjuntos de rpmsg,** siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="bf24d-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="bf24d-104">Conéctese a Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bf24d-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="bf24d-105">Para conectarse a Exchange Online PowerShell, debe iniciar sesión con un administrador global o una cuenta de administrador de Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf24d-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="bf24d-106">a.</span><span class="sxs-lookup"><span data-stu-id="bf24d-106">a.</span></span> <span data-ttu-id="bf24d-107">Abra Windows PowerShell y, a continuación, ejecute el siguiente comando: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="bf24d-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="bf24d-108">b.</span><span class="sxs-lookup"><span data-stu-id="bf24d-108">b.</span></span> <span data-ttu-id="bf24d-109">En el Windows PowerShell de diálogo Solicitud de **credencial,** escriba su cuenta y contraseña de trabajo o escuela, c.</span><span class="sxs-lookup"><span data-stu-id="bf24d-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="bf24d-110">Haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="bf24d-110">Click **OK**.</span></span> 

2. <span data-ttu-id="bf24d-111">Ejecute el siguiente comando para crear una nueva sesión:</span><span class="sxs-lookup"><span data-stu-id="bf24d-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="bf24d-112">a.</span><span class="sxs-lookup"><span data-stu-id="bf24d-112">a.</span></span> <span data-ttu-id="bf24d-113">Ejecute el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="bf24d-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="bf24d-114">Ejecutar `Get-IRMConfiguration` comando.</span><span class="sxs-lookup"><span data-stu-id="bf24d-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="bf24d-115">Compruebe la **configuración ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="bf24d-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="bf24d-116">a.</span><span class="sxs-lookup"><span data-stu-id="bf24d-116">a.</span></span> <span data-ttu-id="bf24d-117">Si **la configuración clientAccessServerEnabled** está establecida en **False,** ejecute el siguiente cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="bf24d-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="bf24d-118">Cierre siempre la sesión de PowerShell con el siguiente comando: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="bf24d-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="bf24d-119">Para obtener más información, [vea Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="bf24d-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

