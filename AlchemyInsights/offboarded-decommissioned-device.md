---
title: Problemas con la eliminación de un dispositivo fuera deborde o retirada del inventario de dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319182"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="48296-102">Problemas con la eliminación de un dispositivo fuera deborde o retirada del inventario de dispositivos</span><span class="sxs-lookup"><span data-stu-id="48296-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="48296-103">Actualmente, Microsoft Defender para endpoint no permite quitar manualmente el registro de dispositivo de un dispositivo fuera deborde o dado de baja del Inventario de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="48296-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="48296-104">Por motivos de seguridad, el dispositivo permanece en el portal como un registro histórico hasta 180 días.</span><span class="sxs-lookup"><span data-stu-id="48296-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="48296-105">Sin embargo, los datos del dispositivo se purgan según el período de retención configurado.</span><span class="sxs-lookup"><span data-stu-id="48296-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="48296-106">**Nota:** Un dispositivo fuera deborde o desmantelado cambia automáticamente al **estado inactivo** después de siete días.</span><span class="sxs-lookup"><span data-stu-id="48296-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="48296-107">Además, los dispositivos que no están activos en los últimos 30 días no se tienen en cuenta en los datos que reflejan la puntuación de exposición de la administración de vulnerabilidades y amenazas de la organización o la puntuación de Microsoft Secure Score para dispositivos.</span><span class="sxs-lookup"><span data-stu-id="48296-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="48296-108">Si aún no quieres ver determinados dispositivos en la vista Inventario de dispositivos, intenta colocar una etiqueta de dispositivo para filtrar el dispositivo dado de baja de la vista Inventario de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="48296-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="48296-109">Para más información, consulte lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="48296-109">For more information, see:</span></span>

[<span data-ttu-id="48296-110">Dispositivos offboard del servicio Microsoft Defender para endpoints</span><span class="sxs-lookup"><span data-stu-id="48296-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="48296-111">Puntuación de exposición en la administración de amenazas y vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="48296-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="48296-112">Corregir sensores incorrectos en Microsoft Defender para endpoint</span><span class="sxs-lookup"><span data-stu-id="48296-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="48296-113">Cómo usar el etiquetado de forma eficaz (parte 1)</span><span class="sxs-lookup"><span data-stu-id="48296-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="48296-114">Cómo usar el etiquetado de forma eficaz (parte 2)</span><span class="sxs-lookup"><span data-stu-id="48296-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="48296-115">Cómo usar el etiquetado de forma eficaz (parte 3)</span><span class="sxs-lookup"><span data-stu-id="48296-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




