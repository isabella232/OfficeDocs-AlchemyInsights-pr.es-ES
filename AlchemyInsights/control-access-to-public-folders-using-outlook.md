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
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar el acceso a las carpetas públicas con Outlook

Para controlar qué usuarios pueden acceder a las carpetas públicas con Outlook:

1. Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook  
$false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook. Este es el valor predeterminado.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: Este procedimiento solo puede controlar las conexiones con la versión de Outlook para escritorio para clientes de Windows. Los usuarios pueden seguir accediendo a las carpetas públicas usando OWA u Outlook para Mac.

Para obtener más información, consulte [Conexiones controladas para las carpetas públicas en Outlook](https://aka.ms/controlpf) para obtener más información.
