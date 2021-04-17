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
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook no puede conectarse a carpetas públicas

Si el acceso a carpetas públicas no funciona para algunos usuarios, pruebe lo siguiente:

Conéctese a EXO PowerShell y configure el parámetro DefaultPublicFolderMailbox en la cuenta de usuario problemática para que coincida con el parámetro en una cuenta de usuario en funcionamiento.

Ejemplo:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Espere al menos una hora para que el cambio entre en vigor.

Si el problema permanece, siga [este procedimiento para](https://aka.ms/pfcte) solucionar problemas de acceso a carpetas públicas con Outlook.
 
**Para controlar qué usuarios pueden tener acceso a carpetas públicas mediante Outlook:**

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false  
      
    $true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook  
      
    $false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook. Este es el valor predeterminado.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Nota** Este procedimiento solo puede controlar las conexiones con el escritorio de Outlook para clientes de Windows. Un usuario puede seguir accediendo a carpetas públicas mediante OWA o Outlook para Mac.
 
Para obtener más información, vea [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).