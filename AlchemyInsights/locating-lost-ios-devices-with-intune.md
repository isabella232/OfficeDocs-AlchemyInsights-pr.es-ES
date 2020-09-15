---
title: Búsqueda de dispositivos iOS perdidos con Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675195"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="72a37-102">Búsqueda de dispositivos iOS perdidos con Intune</span><span class="sxs-lookup"><span data-stu-id="72a37-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="72a37-103">Habilitar el modo de pérdida en un dispositivo iOS permite a un administrador colocar un mensaje y un número de teléfono de contacto en la pantalla de bloqueo del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72a37-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="72a37-104">Después de habilitar el modo de pérdida, el administrador puede usar la acción Buscar dispositivo para identificar la ubicación física del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72a37-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="72a37-105">La acción Buscar dispositivo en Intune funciona con dispositivos iOS, y muestra la ubicación de un dispositivo específico en un mapa.</span><span class="sxs-lookup"><span data-stu-id="72a37-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="72a37-106">El uso de esta acción requiere que el dispositivo iOS esté en:</span><span class="sxs-lookup"><span data-stu-id="72a37-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="72a37-107">Modo supervisado</span><span class="sxs-lookup"><span data-stu-id="72a37-107">Supervised mode</span></span>
- <span data-ttu-id="72a37-108">Modo de pérdida</span><span class="sxs-lookup"><span data-stu-id="72a37-108">Lost mode</span></span>

<span data-ttu-id="72a37-109">Para obtener más información, consulte [Habilitar el modo de pérdida en dispositivos iOS/iPadOS con Intune](https://docs.microsoft.com/intune/device-lost-mode) y [Encontrar dispositivos iOS/iPadOS perdidos o robados, con Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="72a37-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="72a37-110">**Preguntas frecuentes**</span><span class="sxs-lookup"><span data-stu-id="72a37-110">**FAQ**</span></span>

<span data-ttu-id="72a37-111">P: He emitido una acción remota para quitar los datos de la empresa de un dispositivo y ahora se ha quedado en estado pendiente.</span><span class="sxs-lookup"><span data-stu-id="72a37-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="72a37-112">R: Para que una acción remota tenga efecto de forma correcta, el dispositivo de destino debe tener conexión a Internet y estar en buen estado.</span><span class="sxs-lookup"><span data-stu-id="72a37-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="72a37-113">En las siguientes situaciones, la acción remota permanece en estado pendiente durante 30 días o hasta que el dispositivo reconozca el comando:</span><span class="sxs-lookup"><span data-stu-id="72a37-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="72a37-114">Cuando el dispositivo no tiene conectividad</span><span class="sxs-lookup"><span data-stu-id="72a37-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="72a37-115">Cuando el dispositivo deja de tener el estado de administración con Intune.</span><span class="sxs-lookup"><span data-stu-id="72a37-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="72a37-116">Si cree que un dispositivo ya no está protegido y que no podrá eliminar los datos de la empresa, seleccione Eliminar.</span><span class="sxs-lookup"><span data-stu-id="72a37-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="72a37-117">La eliminación borra el registro del dispositivo para que ya no aparezca en la lista de dispositivos de Intune.</span><span class="sxs-lookup"><span data-stu-id="72a37-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="72a37-118">Si el dispositivo se vuelve a activar, el usuario tendrá que volver a inscribirse.</span><span class="sxs-lookup"><span data-stu-id="72a37-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="72a37-119">P: ¿Por qué no puedo usar determinadas acciones remotas?</span><span class="sxs-lookup"><span data-stu-id="72a37-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="72a37-120">R: No todas las plataformas admiten todas las acciones remotas en dispositivos.</span><span class="sxs-lookup"><span data-stu-id="72a37-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="72a37-121">Las siguientes acciones remotas son específicas de una plataforma, por lo que solo están disponibles para las plataformas indicadas.</span><span class="sxs-lookup"><span data-stu-id="72a37-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="72a37-122">Deshabilitar Bloqueo de activación (solo iOS)</span><span class="sxs-lookup"><span data-stu-id="72a37-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="72a37-123">Comienzo de cero (solo Windows)</span><span class="sxs-lookup"><span data-stu-id="72a37-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="72a37-124">Modo perdido (solo iOS)</span><span class="sxs-lookup"><span data-stu-id="72a37-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="72a37-125">Buscar dispositivo (solo iOS)</span><span class="sxs-lookup"><span data-stu-id="72a37-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="72a37-126">Reiniciar (solo Windows)</span><span class="sxs-lookup"><span data-stu-id="72a37-126">Restart (Windows only)</span></span>

<span data-ttu-id="72a37-127">Para obtener más información sobre cada acción, consulte [Acciones de dispositivo disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="72a37-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>