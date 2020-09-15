---
title: Instrucciones para ocultar o mostrar un grupo de la lista de direcciones
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663026"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="4dd85-102">Ocultar grupo de Microsoft 365 de la lista de direcciones (GAL)</span><span class="sxs-lookup"><span data-stu-id="4dd85-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="4dd85-103">Para ocultar un grupo de Microsoft 365 de listas de direcciones (GAL) de clientes de Exchange (como Outlook o OWA), use el comando siguiente en el shell EXO:</span><span class="sxs-lookup"><span data-stu-id="4dd85-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="4dd85-104">Para ocultar el grupo de Microsoft 365 para que no sea visible para los clientes de Exchange, use el comando siguiente en el shell EXO:</span><span class="sxs-lookup"><span data-stu-id="4dd85-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

