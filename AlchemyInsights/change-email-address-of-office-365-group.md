---
title: Cambiar la dirección de correo electrónico de un grupo de Microsoft 365
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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733704"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="022ba-102">Cambiar la dirección de correo electrónico de un grupo de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="022ba-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="022ba-103">Para cambiar la dirección de correo electrónico de un grupo de Microsoft 365, use el Centro de administración.</span><span class="sxs-lookup"><span data-stu-id="022ba-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="022ba-104">Solo tiene que seleccionar el grupo y, luego, seleccionar @editar dirección de correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="022ba-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="022ba-105">También puede usar el siguiente comando de PowerShell EXO para cambiar la dirección SMTP principal de un grupo de Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="022ba-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="022ba-106">Set-UnifiedGroup <Group Name>-PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="022ba-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="022ba-107">Ejemplo:</span><span class="sxs-lookup"><span data-stu-id="022ba-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
