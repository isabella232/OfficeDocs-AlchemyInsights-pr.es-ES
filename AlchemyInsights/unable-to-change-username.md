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
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798681"
---
# <a name="unable-to-change-username"></a>No se puede cambiar el nombre de usuario

En algunos casos, los cambios de UPN (UserPrincipalName) no aparecen en la nube. Es posible que reciba errores de validación en el portal de Office 365 o que no pueda cambiar el nombre de usuario o la dirección de correo electrónico. Para resolver este problema, debe establecer de forma manual el UserPrincipalName con este comando de PowerShell.

**Ejemplo: Cambiar el nombre de usuario**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Este comando cambia el nombre de davidc@contoso.com por davidchew@contoso.com.

Para más información, consulte [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).