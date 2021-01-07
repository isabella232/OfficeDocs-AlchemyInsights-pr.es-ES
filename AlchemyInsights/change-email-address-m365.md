---
title: Cambiar la dirección de correo electrónico de un grupo de Microsoft 365 o Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756574"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Cambiar la dirección de correo electrónico de un grupo de Microsoft 365 o Microsoft Teams

Para cambiar la dirección de correo electrónico de un grupo de Microsoft 365 o Microsoft Teams, use el [Centro de administración de Microsoft 365](https://admin.microsoft.com/). Solo tiene que seleccionar el grupo y, luego, seleccionar @editar dirección de correo electrónico.

También puede usar el siguiente comando de PowerShell EXO para cambiar la dirección SMTP principal de un grupo de Microsoft 365 o de Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Ejemplo:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
