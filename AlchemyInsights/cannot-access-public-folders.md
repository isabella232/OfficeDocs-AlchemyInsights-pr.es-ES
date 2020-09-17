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
      
    $true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook  
      
    $false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook. Este es el valor predeterminado.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Nota:** Este procedimiento puede controlar conexiones solo con el escritorio de Outlook para clientes de Windows. Un usuario puede seguir accediendo a las carpetas públicas mediante OWA o Outlook para Mac.
 
Para obtener más información, vea [anuncio de compatibilidad para conexiones controladas en carpetas públicas en Outlook](https://aka.ms/controlpf).