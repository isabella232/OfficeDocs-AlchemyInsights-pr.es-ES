---
title: Cambiar la de velocidad moderada de EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075914"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="6c839-102">Cambiar la de velocidad moderada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c839-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="6c839-103">Ejecute la prueba automatizada, que le permitirá modificar la directiva de velocidad moderada de EWS durante la migración.</span><span class="sxs-lookup"><span data-stu-id="6c839-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="6c839-104">Tenga en cuenta que, incluso después de que se ejecute, las importaciones EWS seguirán estando limitadas a 150 mb por 5 minutos por buzón; para alcanzar una mayor velocidad de rendimiento de la migración, migre más usuarios a la vez.</span><span class="sxs-lookup"><span data-stu-id="6c839-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="6c839-105">Tenga en cuenta que los cambios en la Directiva de limitación de EWS no tienen efecto en los siguientes tipos de migración (con las herramientas de Microsoft): híbrida, total/preconfigurada (RPC/HTTP), IMAP, G Suite, carpeta pública o servicio de importación de PST.</span><span class="sxs-lookup"><span data-stu-id="6c839-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>