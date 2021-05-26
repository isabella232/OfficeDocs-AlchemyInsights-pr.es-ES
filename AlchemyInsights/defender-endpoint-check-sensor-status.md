---
title: Estado de sensor de Microsoft Defender para punto de conexión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627255"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="465cd-102">Estado de sensor de Microsoft Defender para punto de conexión</span><span class="sxs-lookup"><span data-stu-id="465cd-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="465cd-103">El icono **Dispositivos con problemas de sensores** está en el panel Operaciones de seguridad.</span><span class="sxs-lookup"><span data-stu-id="465cd-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="465cd-104">Este icono proporciona información sobre la capacidad de cada dispositivo de dar datos de sensores y comunicarse con el servicio Microsoft Defender para punto de conexión.</span><span class="sxs-lookup"><span data-stu-id="465cd-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="465cd-105">Indica cuántos dispositivos requieren atención y le ayuda a identificar dispositivos problemáticos y tomar medidas para corregir los problemas conocidos.</span><span class="sxs-lookup"><span data-stu-id="465cd-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="465cd-106">Los dos indicadores de estado del icono dan información sobre el número de dispositivos que no informan correctamente al servicio:</span><span class="sxs-lookup"><span data-stu-id="465cd-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="465cd-107">Dispositivos **mal configurados** que podrían informar parcialmente de datos del sensor al servicio Microsoft Defender para punto de conexión y que podrían tener errores de configuración que deban corregirse.</span><span class="sxs-lookup"><span data-stu-id="465cd-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="465cd-108">**Dispositivos** inactivos que han dejado de informar al servicio Microsoft Defender para punto de conexión durante más de siete días en el mes pasado.</span><span class="sxs-lookup"><span data-stu-id="465cd-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="465cd-109">Al hacer clic en cualquiera de los grupos, se le dirigirá a la lista de dispositivos, filtrada según sus opciones.</span><span class="sxs-lookup"><span data-stu-id="465cd-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="465cd-110">En la lista Dispositivos, puede filtrar la lista de estado según los siguientes estados:</span><span class="sxs-lookup"><span data-stu-id="465cd-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="465cd-111">Dispositivos **activos** que informan de forma activa al servicio Microsoft Defender para punto de conexión.</span><span class="sxs-lookup"><span data-stu-id="465cd-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="465cd-112">Dispositivos **mal configurados** que podrían informar parcialmente de datos del sensor al servicio Microsoft Defender para punto de conexión, pero que tienen errores de configuración que deben corregirse.</span><span class="sxs-lookup"><span data-stu-id="465cd-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="465cd-113">Los dispositivos mal configurados pueden tener uno o varios de los siguientes problemas:</span><span class="sxs-lookup"><span data-stu-id="465cd-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="465cd-114">No hay datos de sensor: los dispositivos han dejado de enviar datos de sensores.</span><span class="sxs-lookup"><span data-stu-id="465cd-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="465cd-115">Se pueden activar alertas limitadas desde el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="465cd-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="465cd-116">Comunicaciones deficientes: la capacidad de comunicarse con el dispositivo es deficiente.</span><span class="sxs-lookup"><span data-stu-id="465cd-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="465cd-117">Puede que el envío de archivos para un análisis profundo, el bloqueo de archivos, el aislamiento de dispositivo de la red y otras acciones que requieran comunicación con el dispositivo no funcionen.</span><span class="sxs-lookup"><span data-stu-id="465cd-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="465cd-118">Dispositivos **inactivos** que han dejado de informar al servicio Microsoft Defender para punto de conexión.</span><span class="sxs-lookup"><span data-stu-id="465cd-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="465cd-119">Puede descargar toda la lista en formato CSV con la característica Exportar.</span><span class="sxs-lookup"><span data-stu-id="465cd-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="465cd-120">Para obtener más información, consulte [Comprobar el estado del sensor en Microsoft Defender para punto de conexión](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="465cd-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="465cd-121">Para obtener más información sobre qué provocó que un dispositivo esté inactivo o mal configurado, vea [Corregir sensores en mal estado en Microsoft Defender para el punto de conexión](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="465cd-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
