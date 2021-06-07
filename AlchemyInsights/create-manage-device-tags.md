---
title: Crear y administrar etiquetas de dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721732"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="31cc7-102">Crear y administrar etiquetas de dispositivos</span><span class="sxs-lookup"><span data-stu-id="31cc7-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="31cc7-103">Agregue etiquetas en los dispositivos para crear una afiliación de grupos lógica.</span><span class="sxs-lookup"><span data-stu-id="31cc7-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="31cc7-104">Las etiquetas de dispositivo son compatibles con la asignación adecuada de la red, lo que permite adjuntar diferentes etiquetas para capturar contexto y habilitar la creación de listas dinámicas como parte de un incidente.</span><span class="sxs-lookup"><span data-stu-id="31cc7-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="31cc7-105">Las etiquetas se pueden usar como filtro en la vista de lista de dispositivos o para agrupar dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31cc7-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="31cc7-106">Para obtener más información sobre la agrupación de dispositivos, consulte [Crear y administrar etiquetas de dispositivo](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="31cc7-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="31cc7-107">Puede agregar etiquetas en dispositivos de varias maneras:</span><span class="sxs-lookup"><span data-stu-id="31cc7-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="31cc7-108">Usando el portal</span><span class="sxs-lookup"><span data-stu-id="31cc7-108">Using the portal</span></span>

- <span data-ttu-id="31cc7-109">Estableciendo un valor de clave de registro</span><span class="sxs-lookup"><span data-stu-id="31cc7-109">Setting a registry key value</span></span>
 
<span data-ttu-id="31cc7-110">**Nota:** Podría haber una latencia entre el momento en que se agrega una etiqueta a un dispositivo y su disponibilidad en la lista de dispositivos y la página de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31cc7-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="31cc7-111">Para agregar etiquetas de dispositivo con la API, consulte [API para agregar o quitar etiquetas de dispositivo](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="31cc7-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="31cc7-112">Agregar y administrar etiquetas de dispositivo con el portal</span><span class="sxs-lookup"><span data-stu-id="31cc7-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="31cc7-113">Seleccione el dispositivo en el que quiere administrar las etiquetas.</span><span class="sxs-lookup"><span data-stu-id="31cc7-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="31cc7-114">Puede seleccionar o buscar un dispositivo desde cualquiera de las siguientes vistas:</span><span class="sxs-lookup"><span data-stu-id="31cc7-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="31cc7-115">**Panel de operaciones de seguridad** Seleccione el nombre del dispositivo en la sección Dispositivos principales con alertas activas.</span><span class="sxs-lookup"><span data-stu-id="31cc7-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="31cc7-116">**Cola de alertas**: seleccione el nombre del dispositivo junto al icono de dispositivo en la cola de alertas.</span><span class="sxs-lookup"><span data-stu-id="31cc7-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="31cc7-117">**Lista de dispositivos**: seleccione el nombre del dispositivo de la lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31cc7-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="31cc7-118">**Cuadro de búsqueda**: seleccione Dispositivo en el menú desplegable y escriba el nombre del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31cc7-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="31cc7-119">También puede acceder a la página de la alerta a través del archivo y las vistas IP.</span><span class="sxs-lookup"><span data-stu-id="31cc7-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="31cc7-120">Seleccione **Administrar etiquetas** en la fila Acciones de respuesta.</span><span class="sxs-lookup"><span data-stu-id="31cc7-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="31cc7-121">Escriba para buscar o crear etiquetas.</span><span class="sxs-lookup"><span data-stu-id="31cc7-121">Type to find or create tags.</span></span>

<span data-ttu-id="31cc7-122">Las etiquetas se agregan a la vista de dispositivo y se reflejan en la vista de lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31cc7-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="31cc7-123">Después podrá usar el filtro etiquetas para ver la lista de dispositivos relevante.</span><span class="sxs-lookup"><span data-stu-id="31cc7-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="31cc7-124">Para obtener más información, consulte [Crear y administrar etiquetas de dispositivo](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="31cc7-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>