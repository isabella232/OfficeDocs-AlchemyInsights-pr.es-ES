---
title: Migrar extensiones de Google Chrome a Microsoft Edge (cromo)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600147"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="5342c-102">Migrar extensiones de Google Chrome a Microsoft Edge (cromo)</span><span class="sxs-lookup"><span data-stu-id="5342c-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="5342c-103">Es fácil [portar las extensiones de Google Chrome a Microsoft Edge (cromo)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="5342c-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="5342c-104">En la mayoría de los casos, solo se necesitan cambios mínimos para ejecutar estas extensiones en Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5342c-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="5342c-105">Las API de extensión y las claves de manifiesto compatibles con Google Chrome son compatibles con el código de Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5342c-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="5342c-106">Sin embargo, Microsoft Edge no es compatible con las API de extensión Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken y Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="5342c-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>