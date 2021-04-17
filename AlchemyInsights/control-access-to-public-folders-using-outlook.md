---
title: Controlar el acceso a las carpetas públicas con Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816757"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar el acceso a las carpetas públicas con Outlook

Para controlar qué usuarios pueden acceder a las carpetas públicas con Outlook:

1. Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Permite que los usuarios tengan acceso a las carpetas públicas en Outlook  
$false: Evita que el usuario tenga acceso a las carpetas públicas en Outlook. Este es el valor predeterminado.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: Este procedimiento solo puede controlar las conexiones con la versión de Outlook para escritorio para clientes de Windows. Los usuarios pueden seguir accediendo a las carpetas públicas usando OWA u Outlook para Mac.

Para obtener más información, consulte [Conexiones controladas para las carpetas públicas en Outlook](https://aka.ms/controlpf) para obtener más información.
