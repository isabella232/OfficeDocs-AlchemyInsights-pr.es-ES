---
title: Inventario de dispositivos Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667895"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="34397-102">Inventario de dispositivos Intune</span><span class="sxs-lookup"><span data-stu-id="34397-102">Intune Device Inventory</span></span>

<span data-ttu-id="34397-103">El blade de dispositivos ofrece a los administradores información acerca de los dispositivos que se administran en Intune por cada uno de estos.</span><span class="sxs-lookup"><span data-stu-id="34397-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="34397-104">La información que se muestra incluye: hardware, aplicaciones detectadas, estado de cumplimiento del dispositivo y estado de configuración del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34397-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="34397-105">Los datos de inventario para el hardware y las aplicaciones detectadas se recopilan en ciclos de siete días.</span><span class="sxs-lookup"><span data-stu-id="34397-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="34397-106">El informe de las aplicaciones y los elementos de hardware específicos es distinto según el sistema operativo del dispositivo y de si el dispositivo es de propiedad personal o empresarial.</span><span class="sxs-lookup"><span data-stu-id="34397-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="34397-107">Para más información, consulte [Ver detalles de dispositivos de Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="34397-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="34397-108">**Preguntas frecuentes**</span><span class="sxs-lookup"><span data-stu-id="34397-108">**FAQ**</span></span>

<span data-ttu-id="34397-109">P: No recibo la lista de inventario completa de las aplicaciones presentes en dispositivos Windows inscritos por Intune.</span><span class="sxs-lookup"><span data-stu-id="34397-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="34397-110">¿Por qué no?</span><span class="sxs-lookup"><span data-stu-id="34397-110">Why not?</span></span>

<span data-ttu-id="34397-111">R: En este momento, solo se muestran las aplicaciones modernas para las PC con Windows 10 que han sido identificadas como dispositivos corporativos.</span><span class="sxs-lookup"><span data-stu-id="34397-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="34397-112">Intune no recopila información sobre las aplicaciones Win32 instaladas en estos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="34397-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="34397-113">P: ¿Por qué no se recopilan los números de teléfono de todos los dispositivos?</span><span class="sxs-lookup"><span data-stu-id="34397-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="34397-114">R: Los teléfonos que presentan categoría de dispositivos corporativos en Intune no se identifican con su número de teléfono completo cuando, por ejemplo, se ejecuta un informe de inventario de dispositivos móviles.</span><span class="sxs-lookup"><span data-stu-id="34397-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="34397-115">Los números de teléfono de dispositivos Bring-your-own-device siempre aparecen de forma parcial con asteriscos (\*\*\*\*), y solo se muestran los últimos cuatro dígitos.</span><span class="sxs-lookup"><span data-stu-id="34397-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>