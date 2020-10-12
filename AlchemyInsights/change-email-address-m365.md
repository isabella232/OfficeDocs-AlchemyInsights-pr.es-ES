---
title: Cambiar la dirección de correo electrónico de grupo de Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416703"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Cambiar la dirección de correo electrónico de un grupo de Microsoft 365

Para cambiar la dirección de correo electrónico de un grupo de Microsoft 365, use el Centro de administración. Solo tiene que seleccionar el grupo y, luego, seleccionar @editar dirección de correo electrónico.

También puede usar el siguiente comando de PowerShell EXO para cambiar la dirección SMTP principal de un grupo de Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Ejemplo:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
