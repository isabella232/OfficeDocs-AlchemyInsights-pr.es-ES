---
title: No se puede tener acceso a las carpetas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341420"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook no puede conectarse a las carpetas públicas

Si el acceso a la carpeta pública no funciona para algunos usuarios, intente lo siguiente:

Conéctese a EXO PowerShell y configure el parámetro DefaultPublicFolderMailbox en la cuenta de usuario problemática para que cumpla el parámetro en una cuenta de usuario que funcione.

Ejemplo:

Get-Mailbox WorkingUser | DefaultPublicFolderMailbox ft, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Espere al menos una hora para que el cambio surta efecto.

Si el problema persiste, siga [este procedimiento](https://aka.ms/pfcte) para solucionar problemas de acceso a carpetas públicas con Outlook.
 
**Para controlar los usuarios que pueden tener acceso a las carpetas públicas mediante Outlook**:

1.  Use set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false  
      
    $true: permitir que los usuarios tengan acceso a carpetas públicas en Outlook  
      
    $false: impedir que el usuario tenga acceso a las carpetas públicas de Outlook. Este es el valor predeterminado.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Nota:** Este procedimiento puede controlar conexiones solo con el escritorio de Outlook para clientes de Windows. Un usuario puede seguir accediendo a las carpetas públicas mediante OWA o Outlook para Mac.
 
Para obtener más información, vea [anuncio de compatibilidad para conexiones controladas en carpetas públicas en Outlook](https://aka.ms/controlpf).