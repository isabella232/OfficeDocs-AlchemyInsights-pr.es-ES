---
title: Instrucciones para ocultar o mostrar el grupo de la lista de direcciones
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
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926262"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ocultar Microsoft 365 de la lista de direcciones (GAL)

Para ocultar un grupo Microsoft 365 de listas de direcciones (GAL) de clientes de Exchange (como Outlook o OWA), use el siguiente comando en el shell EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Para ocultar que el Microsoft 365 está visible para Exchange clientes, use el siguiente comando en el shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

