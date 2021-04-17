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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="65f36-102">Cambiar la dirección de correo electrónico de un grupo de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="65f36-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="65f36-103">Para cambiar la dirección de correo electrónico de un grupo de Microsoft 365, use el Centro de administración.</span><span class="sxs-lookup"><span data-stu-id="65f36-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="65f36-104">Solo tiene que seleccionar el grupo y, luego, seleccionar @editar dirección de correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="65f36-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="65f36-105">También puede usar el siguiente comando de PowerShell EXO para cambiar la dirección SMTP principal de un grupo de Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="65f36-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="65f36-106">Set-UnifiedGroup <Group Name>-PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="65f36-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="65f36-107">Ejemplo:</span><span class="sxs-lookup"><span data-stu-id="65f36-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
