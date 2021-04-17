---
title: Uso de PowerShell para directivas de uso compartido y relaciones de la organización
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
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826072"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="57140-102">Uso de PowerShell para directivas de uso compartido y relaciones de la organización</span><span class="sxs-lookup"><span data-stu-id="57140-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="57140-103">Para las relaciones de la organización, revise la sintaxis detallada y la información de parámetros de: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  Y  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="57140-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="57140-104">Para crear una directiva de uso compartido, use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="57140-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="57140-105">Para [aplicar una directiva de uso compartido a un buzón o a un usuario](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), necesita usar una combinación de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) y [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) con la directiva que acaba de crear.</span><span class="sxs-lookup"><span data-stu-id="57140-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="57140-106">Para [modificar, deshabilitar o quitar una directiva de uso compartido](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) necesita usar [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) y [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="57140-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="57140-107">**Para comprender completamente este tema, lea:**</span><span class="sxs-lookup"><span data-stu-id="57140-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="57140-108">Uso compartido en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="57140-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)