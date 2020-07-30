---
title: No se puede cambiar el nombre de usuario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431823"
---
# <a name="unable-to-change-username"></a>No se puede cambiar el nombre de usuario

En algunos casos, los cambios de UPN (UserPrincipalName) no aparecen en la nube. Es posible que reciba errores de validación en el portal de Office 365 o que no pueda cambiar el nombre de usuario o la dirección de correo electrónico. Para resolver este problema, debe establecer de forma manual el UserPrincipalName con este comando de PowerShell.

**Ejemplo: Cambiar el nombre de usuario**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Este comando cambia el nombre de davidc@contoso.com por davidchew@contoso.com.

Para más información, consulte [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).