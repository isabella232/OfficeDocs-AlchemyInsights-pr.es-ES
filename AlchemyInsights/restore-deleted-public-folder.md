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
# <a name="restore-a-deleted-public-folder"></a>Restaurar una carpeta pública eliminada

**Para restaurar elementos eliminados de una carpeta pública**:

- Vea [no puede recuperar los elementos eliminados de una carpeta pública que no es de correo en Outlook 2016](https://aka.ms/pfrec).
 
**Para restaurar una carpeta pública eliminada (de cualquier tipo)**: 

- Use el siguiente comando de PowerShell EXO:

    Sintaxis:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Ejemplo: en el siguiente comando se restaurará Subfolder1 y se colocará en \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Consulte [restaurar una carpeta pública eliminada](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obtener más información.
