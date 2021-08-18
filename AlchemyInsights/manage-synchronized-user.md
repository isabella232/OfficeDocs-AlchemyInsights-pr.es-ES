---
title: Administrar usuario sincronizado
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114801"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>No se puede establecer la dirección de correo electrónico principal, cambiar los atributos de usuario o quitar o eliminar un usuario sincronizado

Si la sincronización de directorios está habilitada para el entorno, algunos atributos de usuario u objeto no se pueden cambiar mediante el Centro de administración de Microsoft 365.

Para administrar completamente los usuarios sincronizados y todos sus atributos, use la consola de administración de grupos y usuarios de Active Directory local (adsiedit.msc).  

Como alternativa, puede cambiar los usuarios individuales o los atributos de los usuarios sincronizados mediante powershell, como se muestra en estos ejemplos comunes:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
