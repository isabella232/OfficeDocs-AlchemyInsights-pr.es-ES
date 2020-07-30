---
title: No se puede cambiar el nombre de usuario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431823"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="faf00-102">No se puede cambiar el nombre de usuario</span><span class="sxs-lookup"><span data-stu-id="faf00-102">Unable to change UserName</span></span>

<span data-ttu-id="faf00-103">En algunos casos, los cambios de UPN (UserPrincipalName) no aparecen en la nube.</span><span class="sxs-lookup"><span data-stu-id="faf00-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="faf00-104">Es posible que reciba errores de validación en el portal de Office 365 o que no pueda cambiar el nombre de usuario o la dirección de correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="faf00-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="faf00-105">Para resolver este problema, debe establecer de forma manual el UserPrincipalName con este comando de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="faf00-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="faf00-106">**Ejemplo: Cambiar el nombre de usuario**</span><span class="sxs-lookup"><span data-stu-id="faf00-106">**Example: Rename a user**</span></span>

<span data-ttu-id="faf00-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="faf00-107">PowerShellCopy</span></span>

<span data-ttu-id="faf00-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="faf00-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="faf00-109">Este comando cambia el nombre de davidc@contoso.com por davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="faf00-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="faf00-110">Para más información, consulte [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="faf00-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>