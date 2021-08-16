---
title: No se puede cambiar el nombre de usuario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020245"
---
# <a name="unable-to-change-username"></a>No se puede cambiar el nombre de usuario

En algunos casos, los cambios de UPN (UserPrincipalName) no aparecen en la nube. Es posible que reciba errores de validación en el portal de Office 365 o que no pueda cambiar el nombre de usuario o la dirección de correo electrónico. Para resolver este problema, debe establecer de forma manual el UserPrincipalName con este comando de PowerShell.

**Ejemplo: Cambiar el nombre de usuario**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Este comando cambia el nombre de davidc@contoso.com por davidchew@contoso.com.

Para más información, consulte [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).