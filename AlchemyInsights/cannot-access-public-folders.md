---
title: No se puede tener acceso a las carpetas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812564"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="d80d3-102">Outlook no puede conectarse a las carpetas públicas</span><span class="sxs-lookup"><span data-stu-id="d80d3-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="d80d3-103">Si el acceso a la carpeta pública no funciona para algunos usuarios, intente lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d80d3-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="d80d3-104">Conéctese a EXO PowerShell y configure el parámetro DefaultPublicFolderMailbox en la cuenta de usuario problemática para que cumpla el parámetro en una cuenta de usuario que funcione.</span><span class="sxs-lookup"><span data-stu-id="d80d3-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="d80d3-105">Ejemplo:</span><span class="sxs-lookup"><span data-stu-id="d80d3-105">Example:</span></span>

<span data-ttu-id="d80d3-106">Get-Mailbox WorkingUser | DefaultPublicFolderMailbox ft, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="d80d3-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="d80d3-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="d80d3-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="d80d3-108">Espere al menos una hora para que el cambio surta efecto.</span><span class="sxs-lookup"><span data-stu-id="d80d3-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="d80d3-109">Si el problema persiste, siga [este procedimiento](https://aka.ms/pfcte) para solucionar problemas de acceso a carpetas públicas con Outlook.</span><span class="sxs-lookup"><span data-stu-id="d80d3-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="d80d3-110">**Para controlar los usuarios que pueden tener acceso a las carpetas públicas mediante Outlook**:</span><span class="sxs-lookup"><span data-stu-id="d80d3-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="d80d3-111">Use set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false</span><span class="sxs-lookup"><span data-stu-id="d80d3-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="d80d3-112">$true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook</span><span class="sxs-lookup"><span data-stu-id="d80d3-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="d80d3-113">$false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook.</span><span class="sxs-lookup"><span data-stu-id="d80d3-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="d80d3-114">Este es el valor predeterminado.</span><span class="sxs-lookup"><span data-stu-id="d80d3-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="d80d3-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="d80d3-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="d80d3-116">**Nota:** Este procedimiento puede controlar conexiones solo con el escritorio de Outlook para clientes de Windows.</span><span class="sxs-lookup"><span data-stu-id="d80d3-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="d80d3-117">Un usuario puede seguir accediendo a las carpetas públicas mediante OWA o Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="d80d3-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="d80d3-118">Para obtener más información, vea [anuncio de compatibilidad para conexiones controladas en carpetas públicas en Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="d80d3-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>