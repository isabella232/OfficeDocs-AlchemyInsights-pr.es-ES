---
title: Retirada de herramientas de exhibición de documentos electrónicos heredadas
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798566"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="d09a4-102">Retirada de herramientas de exhibición de documentos electrónicos heredadas</span><span class="sxs-lookup"><span data-stu-id="d09a4-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="d09a4-103">Como resultado de la nueva y mejorada funcionalidad de exhibición de documentos electrónicos en el Centro de cumplimiento de Microsoft 365, las siguientes herramientas y comandos heredados de exhibición de documentos electrónicos se retirarán en los próximos meses:</span><span class="sxs-lookup"><span data-stu-id="d09a4-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="d09a4-104">[Exhibición de documentos electrónicos](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) local [y](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) retenciones locales en el Centro de administración de Exchange.</span><span class="sxs-lookup"><span data-stu-id="d09a4-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="d09a4-105">Los cmdlets de PowerShell de Exchange Online que admiten In-Place eDiscovery y In-Place holds.</span><span class="sxs-lookup"><span data-stu-id="d09a4-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="d09a4-106">(Estos cmdlets se identifican colectivamente como cmdlets \*-MailboxSearch). Esto incluye los cmdlets siguientes:</span><span class="sxs-lookup"><span data-stu-id="d09a4-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="d09a4-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d09a4-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="d09a4-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d09a4-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="d09a4-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d09a4-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="d09a4-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d09a4-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="d09a4-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) en Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d09a4-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="d09a4-112">Las siguientes operaciones en la API de servicios web de Exchange:</span><span class="sxs-lookup"><span data-stu-id="d09a4-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="d09a4-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d09a4-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="d09a4-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d09a4-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="d09a4-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d09a4-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="d09a4-116">EDiscovery avanzada v1.0</span><span class="sxs-lookup"><span data-stu-id="d09a4-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="d09a4-117">**Escala de tiempo para la retirada:**</span><span class="sxs-lookup"><span data-stu-id="d09a4-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="d09a4-118">**1 de julio de 2020** Ya no puede crear nuevas búsquedas y retenciones, pero puede ejecutar, editar y eliminar búsquedas existentes bajo su propio riesgo.</span><span class="sxs-lookup"><span data-stu-id="d09a4-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="d09a4-119">El soporte técnico de Microsoft ya no admite In-Place de exhibición & de documentos electrónicos en el EAC.</span><span class="sxs-lookup"><span data-stu-id="d09a4-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="d09a4-120">1 de octubre de **2020In-Place** la funcionalidad de exhibición de documentos electrónicos & en el EAC se colocará en modo de solo lectura, por lo que solo puede quitar las búsquedas y retenciones existentes.</span><span class="sxs-lookup"><span data-stu-id="d09a4-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="d09a4-121">**Para obtener más información, vea**:</span><span class="sxs-lookup"><span data-stu-id="d09a4-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="d09a4-122">Migrar búsquedas y retenciones de exhibición de documentos electrónicos heredados al Centro de cumplimiento de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d09a4-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="d09a4-123">Retirada de herramientas heredadas de eDiscovery</span><span class="sxs-lookup"><span data-stu-id="d09a4-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="d09a4-124">Preguntas frecuentes sobre In-Place eDiscovery y In-Place holds</span><span class="sxs-lookup"><span data-stu-id="d09a4-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



