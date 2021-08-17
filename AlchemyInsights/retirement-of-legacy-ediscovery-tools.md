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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074697"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retirada de herramientas de exhibición de documentos electrónicos heredadas

Como resultado de la nueva y mejorada funcionalidad de exhibición de documentos electrónicos en el Centro de cumplimiento de Microsoft 365, las siguientes herramientas y comandos heredados de exhibición de documentos electrónicos se retirarán en los próximos meses:

- [Exhibición de](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) documentos [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) electrónicos local y retenciones locales en el centro Exchange administración local.

- Los Exchange Online de PowerShell que admiten In-Place eDiscovery y In-Place holds. (Estos cmdlets se identifican colectivamente como cmdlets *-MailboxSearch). Esto incluye los cmdlets siguientes:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- El [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) en Exchange Online PowerShell.
- Las siguientes operaciones en la API Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Escala de tiempo para la retirada:**
- **1 de julio de 2020** Ya no puede crear nuevas búsquedas y retenciones, pero puede ejecutar, editar y eliminar búsquedas existentes bajo su propio riesgo. El soporte técnico de Microsoft ya no admite In-Place de exhibición & de documentos electrónicos en el EAC.
    
- 1 de octubre de **2020In-Place** la funcionalidad de exhibición de documentos electrónicos & en el EAC se colocará en modo de solo lectura, por lo que solo puede quitar las búsquedas y retenciones existentes.

**Para obtener más información, vea**:

 - [Migrar búsquedas y retenciones de exhibición de documentos electrónicos heredados a la Centro de cumplimiento de Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retirada de herramientas heredadas de eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Preguntas frecuentes sobre In-Place eDiscovery y In-Place holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



