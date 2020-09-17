---
title: Ocultar o mostrar equipos o grupos de Office 365 de la lista de direcciones
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
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782344"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="ee8f7-102">Ocultar o mostrar equipos o grupos de Office 365 de la lista de direcciones</span><span class="sxs-lookup"><span data-stu-id="ee8f7-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="ee8f7-103">Use el siguiente comando de PowerShell EXO para ocultar o mostrar equipos o grupos de Office 365 de las listas de direcciones (GAL) de los clientes de Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="ee8f7-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="ee8f7-104">Use el siguiente comando de PowerShell EXO para ocultar o mostrar equipos o grupos de Office 365 de los clientes de Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="ee8f7-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="ee8f7-105">Para obtener instrucciones detalladas, consulte [Ocultar Grupos de Office 365 desde la GAL y los clientes de Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="ee8f7-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
