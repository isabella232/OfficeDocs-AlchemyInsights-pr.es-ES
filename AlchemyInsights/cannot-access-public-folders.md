---
title: No se puede acceder a carpetas públicas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819529"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="6a4ae-102">Outlook no puede conectarse a carpetas públicas</span><span class="sxs-lookup"><span data-stu-id="6a4ae-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="6a4ae-103">Si el acceso a carpetas públicas no funciona para algunos usuarios, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="6a4ae-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="6a4ae-104">Conéctese a EXO PowerShell y configure el parámetro DefaultPublicFolderMailbox en la cuenta de usuario problemática para que coincida con el parámetro en una cuenta de usuario en funcionamiento.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="6a4ae-105">Ejemplo:</span><span class="sxs-lookup"><span data-stu-id="6a4ae-105">Example:</span></span>

<span data-ttu-id="6a4ae-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="6a4ae-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="6a4ae-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="6a4ae-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="6a4ae-108">Espere al menos una hora para que el cambio entre en vigor.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="6a4ae-109">Si el problema permanece, siga [este procedimiento para](https://aka.ms/pfcte) solucionar problemas de acceso a carpetas públicas con Outlook.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="6a4ae-110">**Para controlar qué usuarios pueden tener acceso a carpetas públicas mediante Outlook:**</span><span class="sxs-lookup"><span data-stu-id="6a4ae-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="6a4ae-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false</span><span class="sxs-lookup"><span data-stu-id="6a4ae-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="6a4ae-112">$true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook</span><span class="sxs-lookup"><span data-stu-id="6a4ae-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="6a4ae-113">$false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="6a4ae-114">Este es el valor predeterminado.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="6a4ae-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="6a4ae-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="6a4ae-116">**Nota** Este procedimiento solo puede controlar las conexiones con el escritorio de Outlook para clientes de Windows.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="6a4ae-117">Un usuario puede seguir accediendo a carpetas públicas mediante OWA o Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="6a4ae-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="6a4ae-118">Para obtener más información, vea [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="6a4ae-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>