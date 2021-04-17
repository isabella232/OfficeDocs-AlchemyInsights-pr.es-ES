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
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823984"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="66c2e-102">No se puede establecer la dirección de correo electrónico principal, cambiar los atributos de usuario o quitar o eliminar un usuario sincronizado</span><span class="sxs-lookup"><span data-stu-id="66c2e-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="66c2e-103">Si la sincronización de directorios está habilitada para su entorno, algunos atributos de usuario u objeto no se pueden cambiar con el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="66c2e-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="66c2e-104">Para administrar completamente los usuarios sincronizados y todos sus atributos, use la consola de administración de grupos y usuarios de Active Directory local (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="66c2e-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="66c2e-105">Como alternativa, puede cambiar los usuarios individuales o los atributos de los usuarios sincronizados mediante powershell, como se muestra en estos ejemplos comunes:</span><span class="sxs-lookup"><span data-stu-id="66c2e-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
