---
title: Restaurar una carpeta pública eliminada
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809456"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurar una carpeta pública eliminada

**Para restaurar elementos eliminados de una carpeta pública:**

- Vea [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).
 
**Para restaurar una carpeta pública eliminada (de cualquier tipo):** 

- Use el siguiente comando exo de PowerShell:

    Sintaxis:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Ejemplo: el siguiente comando restaurará Subcarpeta1 y lo colocará en \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Consulta [Restaurar una carpeta pública eliminada para](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) obtener más información.
