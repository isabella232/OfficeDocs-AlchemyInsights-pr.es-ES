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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943392"
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
