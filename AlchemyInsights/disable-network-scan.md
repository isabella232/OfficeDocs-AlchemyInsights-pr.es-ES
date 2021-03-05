---
title: Deshabilitar el examen de red
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449159"
---
# <a name="disable-network-scan"></a><span data-ttu-id="2d244-102">Deshabilitar el examen de red</span><span class="sxs-lookup"><span data-stu-id="2d244-102">Disable network scan</span></span>

<span data-ttu-id="2d244-103">Los exámenes de recursos compartidos de red pueden afectar al rendimiento.</span><span class="sxs-lookup"><span data-stu-id="2d244-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="2d244-104">Para asegurarse de que el cliente no analiza recursos compartidos o archivos de red de forma predeterminada, configure las siguientes opciones en la aplicación Windows Defender en **True**:</span><span class="sxs-lookup"><span data-stu-id="2d244-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="2d244-105">DisableScanningMappedNetworkDrivesForFullScan</span><span class="sxs-lookup"><span data-stu-id="2d244-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="2d244-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="2d244-106">DisableScanningNetworkFiles</span></span>