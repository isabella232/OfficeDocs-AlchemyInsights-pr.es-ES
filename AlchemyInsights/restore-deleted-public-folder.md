---
title: Restaurar una carpeta pública eliminada
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774548"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="88f52-102">Restaurar una carpeta pública eliminada</span><span class="sxs-lookup"><span data-stu-id="88f52-102">Restore a deleted public folder</span></span>

<span data-ttu-id="88f52-103">**Para restaurar elementos eliminados de una carpeta pública**:</span><span class="sxs-lookup"><span data-stu-id="88f52-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="88f52-104">Vea [no puede recuperar los elementos eliminados de una carpeta pública que no es de correo en Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="88f52-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="88f52-105">**Para restaurar una carpeta pública eliminada (de cualquier tipo)**:</span><span class="sxs-lookup"><span data-stu-id="88f52-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="88f52-106">Use el siguiente comando de PowerShell EXO:</span><span class="sxs-lookup"><span data-stu-id="88f52-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="88f52-107">Sintaxis:</span><span class="sxs-lookup"><span data-stu-id="88f52-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="88f52-108">Ejemplo: en el siguiente comando se restaurará Subfolder1 y se colocará en \Parent1:</span><span class="sxs-lookup"><span data-stu-id="88f52-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="88f52-109">Consulte [restaurar una carpeta pública eliminada](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="88f52-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
