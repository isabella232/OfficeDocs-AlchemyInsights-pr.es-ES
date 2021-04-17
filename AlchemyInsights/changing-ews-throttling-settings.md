---
title: Cambiar la de velocidad moderada de EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818053"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="8f81b-102">Cambiar la de velocidad moderada de EWS</span><span class="sxs-lookup"><span data-stu-id="8f81b-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="8f81b-103">Ejecute la prueba automatizada, que le permitirá modificar la directiva de velocidad moderada de EWS durante la migración.</span><span class="sxs-lookup"><span data-stu-id="8f81b-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="8f81b-104">Tenga en cuenta que, incluso después de que se ejecute, las importaciones EWS seguirán estando limitadas a 150 mb por 5 minutos por buzón; para alcanzar una mayor velocidad de rendimiento de la migración, migre más usuarios a la vez.</span><span class="sxs-lookup"><span data-stu-id="8f81b-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="8f81b-105">Tenga en cuenta que los cambios en la Directiva de limitación de EWS no tienen efecto en los siguientes tipos de migración (con las herramientas de Microsoft): híbrida, total/preconfigurada (RPC/HTTP), IMAP, G Suite, carpeta pública o servicio de importación de PST.</span><span class="sxs-lookup"><span data-stu-id="8f81b-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>