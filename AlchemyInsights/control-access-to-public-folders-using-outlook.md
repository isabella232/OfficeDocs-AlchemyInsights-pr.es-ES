---
title: Controlar el acceso a las carpetas públicas con Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816757"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="ded70-102">Controlar el acceso a las carpetas públicas con Outlook</span><span class="sxs-lookup"><span data-stu-id="ded70-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="ded70-103">Para controlar qué usuarios pueden acceder a las carpetas públicas con Outlook:</span><span class="sxs-lookup"><span data-stu-id="ded70-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="ded70-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="ded70-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="ded70-105">$true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook</span><span class="sxs-lookup"><span data-stu-id="ded70-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="ded70-106">$false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook.</span><span class="sxs-lookup"><span data-stu-id="ded70-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ded70-107">Este es el valor predeterminado.</span><span class="sxs-lookup"><span data-stu-id="ded70-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="ded70-108">Nota: Este procedimiento solo puede controlar las conexiones con la versión de Outlook para escritorio para clientes de Windows.</span><span class="sxs-lookup"><span data-stu-id="ded70-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ded70-109">Los usuarios pueden seguir accediendo a las carpetas públicas usando OWA u Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="ded70-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="ded70-110">Para obtener más información, consulte [Conexiones controladas para las carpetas públicas en Outlook](https://aka.ms/controlpf) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="ded70-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
