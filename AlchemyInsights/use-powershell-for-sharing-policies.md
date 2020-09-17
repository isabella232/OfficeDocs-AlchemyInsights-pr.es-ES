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
ms.openlocfilehash: 378dedb332ced2c86899401c54726eb6b7e25d08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773432"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Uso de PowerShell para directivas de uso compartido y relaciones de la organización


Para las relaciones de la organización, revise la sintaxis detallada y la información de parámetros de: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  Y  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Para crear una directiva de uso compartido, use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Para [aplicar una directiva de uso compartido a un buzón o a un usuario](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), necesita usar una combinación de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) y [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) con la directiva que acaba de crear. Para [modificar, deshabilitar o quitar una directiva de uso compartido](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) necesita usar [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) y [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Para comprender completamente este tema, lea:**

[Uso compartido en Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)