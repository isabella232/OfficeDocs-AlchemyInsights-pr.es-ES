---
title: Uso de PowerShell para directivas de uso compartido y relaciones de la organización
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
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709483"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="24fe7-102">Uso de PowerShell para directivas de uso compartido y relaciones de la organización</span><span class="sxs-lookup"><span data-stu-id="24fe7-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="24fe7-103">Para las relaciones de la organización, revise la sintaxis detallada y la información de parámetros de: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  Y  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="24fe7-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="24fe7-104">Para crear una directiva de uso compartido, use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="24fe7-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="24fe7-105">Para [aplicar una directiva de uso compartido a un buzón o a un usuario](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), necesita usar una combinación de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) y [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) con la directiva que acaba de crear.</span><span class="sxs-lookup"><span data-stu-id="24fe7-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="24fe7-106">Para [modificar, deshabilitar o quitar una directiva de uso compartido](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) necesita usar [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) y [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="24fe7-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="24fe7-107">**Para comprender completamente este tema, lea:**</span><span class="sxs-lookup"><span data-stu-id="24fe7-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="24fe7-108">Uso compartido en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="24fe7-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)