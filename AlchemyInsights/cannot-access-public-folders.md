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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996647"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook conectarse a carpetas públicas

Si el acceso a carpetas públicas no funciona para algunos usuarios, pruebe lo siguiente:

Conectar a EXO PowerShell y configure el parámetro DefaultPublicFolderMailbox en la cuenta de usuario problemática para que coincida con el parámetro en una cuenta de usuario en funcionamiento.

Ejemplo:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Espere al menos una hora para que el cambio entre en vigor.

Si el problema permanece, siga [este procedimiento para](https://aka.ms/pfcte) solucionar problemas de acceso a carpetas públicas mediante Outlook.
 
**Para controlar qué usuarios pueden tener acceso a carpetas públicas mediante Outlook**:

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false  
      
    $true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook  
      
    $false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook. Este es el valor predeterminado.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Nota** Este procedimiento solo puede controlar las conexiones Outlook escritorio para Windows clientes. Un usuario puede seguir teniendo acceso a carpetas públicas mediante OWA o Outlook para Mac.
 
Para obtener más información, consulta Anuncio de compatibilidad para [conexiones controladas](https://aka.ms/controlpf)a carpetas públicas en Outlook .