---
title: Cambiar la dirección de correo electrónico de un grupo de Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580674"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Cambiar la dirección de correo electrónico de un grupo de Microsoft 365

Para cambiar la dirección de correo electrónico de un grupo de Microsoft 365, use el Centro de administración. Solo tiene que seleccionar el grupo y, luego, seleccionar @editar dirección de correo electrónico.

También puede usar el siguiente comando de PowerShell EXO para cambiar la dirección SMTP principal de un grupo de Microsoft 365:

Set-UnifiedGroup <Group Name>-PrimarySmtpAddress <new SMTP Address>

Ejemplo:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
