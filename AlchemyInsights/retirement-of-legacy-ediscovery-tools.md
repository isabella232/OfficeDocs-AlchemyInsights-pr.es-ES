---
title: Retirada de herramientas de eDiscovery heredadas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902637"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="04553-102">Retirada de herramientas de eDiscovery heredadas</span><span class="sxs-lookup"><span data-stu-id="04553-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="04553-103">Como resultado de la nueva y mejorada funcionalidad de eDiscovery en el centro de cumplimiento de Microsoft 365, las siguientes herramientas y commandlets de eDiscovery heredadas se retirarán en los próximos meses:</span><span class="sxs-lookup"><span data-stu-id="04553-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="04553-104">[Exhibición](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) de documentos electrónicos local y [conservaciones locales](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) en el centro de administración de Exchange.</span><span class="sxs-lookup"><span data-stu-id="04553-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="04553-105">Los cmdlets de PowerShell de Exchange online que admiten la exhibición de documentos electrónicos local y las suspensiones locales.</span><span class="sxs-lookup"><span data-stu-id="04553-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="04553-106">(Estos cmdlets se identifican colectivamente como cmdlets \*-MailboxSearch). Esto incluye los siguientes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="04553-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="04553-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="04553-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="04553-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="04553-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="04553-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="04553-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="04553-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="04553-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="04553-111">El cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) en Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="04553-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="04553-112">Las siguientes operaciones en la API de servicios web Exchange:</span><span class="sxs-lookup"><span data-stu-id="04553-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="04553-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="04553-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="04553-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="04553-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="04553-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="04553-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="04553-116">EDiscovery avanzado v 1.0</span><span class="sxs-lookup"><span data-stu-id="04553-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="04553-117">**Escala de tiempo para la jubilación**:</span><span class="sxs-lookup"><span data-stu-id="04553-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="04553-118">**1 de julio de 2020** Ya no puede crear nuevas búsquedas ni suspensiones, pero puede ejecutar, editar y eliminar las búsquedas existentes bajo su propio riesgo.</span><span class="sxs-lookup"><span data-stu-id="04553-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="04553-119">El soporte técnico de Microsoft ya no admite la exhibición de documentos electrónicos local & retenciones en el EAC.</span><span class="sxs-lookup"><span data-stu-id="04553-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="04553-120">**1 de octubre de 2020** La exhibición de documentos electrónicos local & mantiene la funcionalidad en el EAC se colocará en modo de solo lectura, por lo que solo podrá quitar búsquedas y suspensiones existentes.</span><span class="sxs-lookup"><span data-stu-id="04553-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="04553-121">**Para obtener más información, vea**:</span><span class="sxs-lookup"><span data-stu-id="04553-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="04553-122">Migrar las búsquedas y suspensiones de eDiscovery heredado al centro de cumplimiento de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="04553-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="04553-123">Retirada de herramientas heredadas de eDiscovery</span><span class="sxs-lookup"><span data-stu-id="04553-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="04553-124">Preguntas más frecuentes sobre la exhibición de documentos electrónicos local y las suspensiones locales</span><span class="sxs-lookup"><span data-stu-id="04553-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



