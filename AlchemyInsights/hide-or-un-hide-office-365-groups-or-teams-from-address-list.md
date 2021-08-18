---
title: Ocultar o mostrar equipos o grupos de Office 365 de la lista de direcciones
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
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088413"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ocultar o mostrar equipos o grupos de Office 365 de la lista de direcciones

Use el siguiente comando de PowerShell EXO para ocultar o mostrar equipos o grupos de Office 365 de las listas de direcciones (GAL) de los clientes de Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Use el siguiente comando de PowerShell EXO para ocultar o mostrar equipos o grupos de Office 365 de los clientes de Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Para obtener instrucciones detalladas, consulte [Ocultar Grupos de Office 365 desde la GAL y los clientes de Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
