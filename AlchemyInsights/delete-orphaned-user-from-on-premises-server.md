---
title: Eliminar usuario huérfano del servidor local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186152"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="04d2a-102">Eliminar usuario huérfano del servidor local</span><span class="sxs-lookup"><span data-stu-id="04d2a-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="04d2a-103">Para quitar un usuario huérfano, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="04d2a-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="04d2a-104">Fuerce la sincronización de directorios siguiendo las instrucciones en [¿Qué es la identidad híbrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="04d2a-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="04d2a-105">Para comprobar la sincronización de directorios, consulte [¿Qué es la identidad híbrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="04d2a-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="04d2a-106">Si las funciones de sincronización son correctas pero la eliminación de objetos de Active Directory no se propaga a Azure AD, elimine manualmente el objeto huérfano mediante uno de los siguientes cmdlets del Módulo Azure Active Directory para Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="04d2a-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="04d2a-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="04d2a-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="04d2a-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="04d2a-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="04d2a-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="04d2a-109">Remove-MsolUser</span></span>

    <span data-ttu-id="04d2a-110">Por ejemplo, para quitar el Id. de usuario huérfano iker.arteaga@contoso.com, creado originalmente con la sincronización de directorios, ejecute el cmdlet:</span><span class="sxs-lookup"><span data-stu-id="04d2a-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="04d2a-111">Remove-MsolUser –UserPrincipalName Iker.Arteaga@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="04d2a-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>