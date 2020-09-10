---
title: Controlar el acceso a las carpetas públicas con Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406611"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="e57e3-102">Controlar el acceso a las carpetas públicas con Outlook</span><span class="sxs-lookup"><span data-stu-id="e57e3-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="e57e3-103">Para controlar qué usuarios pueden acceder a las carpetas públicas con Outlook:</span><span class="sxs-lookup"><span data-stu-id="e57e3-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="e57e3-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="e57e3-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="e57e3-105">$true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook</span><span class="sxs-lookup"><span data-stu-id="e57e3-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="e57e3-106">$false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook.</span><span class="sxs-lookup"><span data-stu-id="e57e3-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e57e3-107">Este es el valor predeterminado.</span><span class="sxs-lookup"><span data-stu-id="e57e3-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="e57e3-108">Nota: Este procedimiento solo puede controlar las conexiones con la versión de Outlook para escritorio para clientes de Windows.</span><span class="sxs-lookup"><span data-stu-id="e57e3-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e57e3-109">Los usuarios pueden seguir accediendo a las carpetas públicas usando OWA u Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="e57e3-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="e57e3-110">Para obtener más información, consulte [Conexiones controladas para las carpetas públicas en Outlook](https://aka.ms/controlpf) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="e57e3-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
