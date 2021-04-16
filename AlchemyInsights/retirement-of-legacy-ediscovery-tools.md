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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retirada de herramientas de exhibición de documentos electrónicos heredadas

Como resultado de la nueva y mejorada funcionalidad de exhibición de documentos electrónicos en el Centro de cumplimiento de Microsoft 365, las siguientes herramientas y comandos heredados de exhibición de documentos electrónicos se retirarán en los próximos meses:

- [Exhibición de documentos electrónicos](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) local [y](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) retenciones locales en el Centro de administración de Exchange.

- Los cmdlets de PowerShell de Exchange Online que admiten In-Place eDiscovery y In-Place holds. (Estos cmdlets se identifican colectivamente como cmdlets *-MailboxSearch). Esto incluye los cmdlets siguientes:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) en Exchange Online PowerShell.
- Las siguientes operaciones en la API de servicios web de Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [EDiscovery avanzada v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Escala de tiempo para la retirada:**
- **1 de julio de 2020** Ya no puede crear nuevas búsquedas y retenciones, pero puede ejecutar, editar y eliminar búsquedas existentes bajo su propio riesgo. El soporte técnico de Microsoft ya no admite In-Place de exhibición & de documentos electrónicos en el EAC.
    
- 1 de octubre de **2020In-Place** la funcionalidad de exhibición de documentos electrónicos & en el EAC se colocará en modo de solo lectura, por lo que solo puede quitar las búsquedas y retenciones existentes.

**Para obtener más información, vea**:

 - [Migrar búsquedas y retenciones de exhibición de documentos electrónicos heredados al Centro de cumplimiento de Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retirada de herramientas heredadas de eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Preguntas frecuentes sobre In-Place eDiscovery y In-Place holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



