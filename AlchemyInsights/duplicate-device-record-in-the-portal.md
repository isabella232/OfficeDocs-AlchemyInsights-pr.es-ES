---
title: Registro duplicado de dispositivo en el portal
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814533"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="baf7a-102">Registro duplicado de dispositivo en el portal</span><span class="sxs-lookup"><span data-stu-id="baf7a-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="baf7a-103">Es posible que vea dos registros de un mismo dispositivo en el portal si el dispositivo no ha informado correctamente del estado de administración conjunta en el sitio de Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="baf7a-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="baf7a-104">Para comprobar el estado de administración conjunta de un dispositivo, revise la columna **Administrado conjuntamente** del dispositivo en la consola de Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="baf7a-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="baf7a-105">Si la columna no está visible, puede agregarla haciendo clic con el botón derecho en cualquiera de los encabezados de columna y seleccionándola en la lista.</span><span class="sxs-lookup"><span data-stu-id="baf7a-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="baf7a-106">El valor de administración conjunta tiene que ser **Sí**.</span><span class="sxs-lookup"><span data-stu-id="baf7a-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="baf7a-107">Si el valor es **No**, abra el applet de cliente de Configuration Manager en el dispositivo cliente y compruebe la propiedad **Administración conjunta** en la pestaña General.</span><span class="sxs-lookup"><span data-stu-id="baf7a-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="baf7a-108">Si el valor es **Habilitado**, existen problemas con la comunicación del cliente con el punto de administración.</span><span class="sxs-lookup"><span data-stu-id="baf7a-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="baf7a-109">Revise **CcmMessaging.log** en el dispositivo para investigar posibles problemas de conectividad.</span><span class="sxs-lookup"><span data-stu-id="baf7a-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="baf7a-110">Si el valor es **Deshabilitado** y el dispositivo está inscrito en Intune, revise **CoManagementHandler.log** en el dispositivo para asegurarse de que el dispositivo ha recibido la Directiva de administración conjunta.</span><span class="sxs-lookup"><span data-stu-id="baf7a-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
