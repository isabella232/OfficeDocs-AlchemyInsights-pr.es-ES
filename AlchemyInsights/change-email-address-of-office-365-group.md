---
title: Cambiar la dirección de correo electrónico de un grupo de Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819061"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Cambiar la dirección de correo electrónico de un grupo de Microsoft 365

Para cambiar la dirección de correo electrónico de un grupo de Microsoft 365, use el Centro de administración. Solo tiene que seleccionar el grupo y, luego, seleccionar @editar dirección de correo electrónico.

También puede usar el siguiente comando de PowerShell EXO para cambiar la dirección SMTP principal de un grupo de Microsoft 365:

Set-UnifiedGroup <Group Name>-PrimarySmtpAddress <new SMTP Address>

Ejemplo:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
