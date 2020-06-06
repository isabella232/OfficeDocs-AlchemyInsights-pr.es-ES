---
title: Instrucciones para ocultar o mostrar un grupo de la lista de direcciones
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580026"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="758ee-102">Ocultar grupo de Microsoft 365 de la lista de direcciones (GAL)</span><span class="sxs-lookup"><span data-stu-id="758ee-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="758ee-103">Para ocultar un grupo de Microsoft 365 de listas de direcciones (GAL) de clientes de Exchange (como Outlook o OWA), use el comando siguiente en el shell EXO:</span><span class="sxs-lookup"><span data-stu-id="758ee-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="758ee-104">Para ocultar el grupo de Microsoft 365 para que no sea visible para los clientes de Exchange, use el comando siguiente en el shell EXO:</span><span class="sxs-lookup"><span data-stu-id="758ee-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

