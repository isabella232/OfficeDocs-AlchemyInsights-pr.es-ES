---
title: Deshabilitar el bloqueo de activación en dispositivos iOS controlados con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397761"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="61b65-102">Deshabilitar el bloqueo de activación en dispositivos iOS controlados con Intune</span><span class="sxs-lookup"><span data-stu-id="61b65-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="61b65-103">La capacidad de deshabilitar el bloqueo de activación en dispositivos iOS facilita la recuperación en el caso en que un usuario habilite el bloqueo de activación en un dispositivo corporativo, y luego abandone la empresa.</span><span class="sxs-lookup"><span data-stu-id="61b65-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="61b65-104">Los requisitos previos para deshabilitar un bloqueo de activación son los siguientes:</span><span class="sxs-lookup"><span data-stu-id="61b65-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="61b65-105">Un dispositivo que se "supervisa".</span><span class="sxs-lookup"><span data-stu-id="61b65-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="61b65-106">El bloqueo de activación se habilitó correctamente con la directiva de restricción de dispositivos iOS en Intune.</span><span class="sxs-lookup"><span data-stu-id="61b65-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="61b65-107">Asimismo, al deshabilitar un bloqueo de activación, debe:</span><span class="sxs-lookup"><span data-stu-id="61b65-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="61b65-108">Poseer físicamente el dispositivo que se va a borrar.</span><span class="sxs-lookup"><span data-stu-id="61b65-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="61b65-109">Copiar el código antes de emitir el borrado.</span><span class="sxs-lookup"><span data-stu-id="61b65-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="61b65-110">**Nota:** el código de borrado no distingue entre mayúsculas y minúsculas, por lo que los caracteres "-" no son necesarios.</span><span class="sxs-lookup"><span data-stu-id="61b65-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="61b65-111">Para obtener más información, consulte [Deshabilitar el bloqueo de activación en dispositivos iOS supervisados con Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="61b65-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="61b65-112">**Preguntas frecuentes**</span><span class="sxs-lookup"><span data-stu-id="61b65-112">**FAQ**</span></span>

<span data-ttu-id="61b65-113">P: **He emitido una acción remota para quitar los datos de la empresa de un dispositivo y ahora está atascado en un estado pendiente.**</span><span class="sxs-lookup"><span data-stu-id="61b65-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="61b65-114">R: Para que una acción remota finalice correctamente, el dispositivo de destino tiene que estar conectado y en buen estado.</span><span class="sxs-lookup"><span data-stu-id="61b65-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="61b65-115">En las siguientes situaciones, la acción remota permanece en un estado pendiente durante 30 días o hasta que el dispositivo reconozca el comando cuando:</span><span class="sxs-lookup"><span data-stu-id="61b65-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="61b65-116">No tiene conectividad.</span><span class="sxs-lookup"><span data-stu-id="61b65-116">Does not have connectivity.</span></span>
- <span data-ttu-id="61b65-117">Pierde su estado de administración con Intune.</span><span class="sxs-lookup"><span data-stu-id="61b65-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="61b65-118">Si cree que un dispositivo ya no se está comprobando, y que no se quitarán los datos de la empresa, seleccione Eliminar.</span><span class="sxs-lookup"><span data-stu-id="61b65-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="61b65-119">La eliminación quita el registro del dispositivo para que ya no aparezca en la lista de dispositivos de Intune.</span><span class="sxs-lookup"><span data-stu-id="61b65-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="61b65-120">Para volver a activar el dispositivo, el usuario debe volverlo a inscribir.</span><span class="sxs-lookup"><span data-stu-id="61b65-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="61b65-121">P: **¿Por qué no puedo usar determinadas acciones remotas?**</span><span class="sxs-lookup"><span data-stu-id="61b65-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="61b65-122">R: No todas las plataformas admiten todas las acciones remotas en dispositivos.</span><span class="sxs-lookup"><span data-stu-id="61b65-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="61b65-123">Las siguientes acciones remotas son específicas para cada plataforma.</span><span class="sxs-lookup"><span data-stu-id="61b65-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="61b65-124">Deshabilitar Bloqueo de activación (solo iOS)</span><span class="sxs-lookup"><span data-stu-id="61b65-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="61b65-125">Comienzo de cero (solo Windows)</span><span class="sxs-lookup"><span data-stu-id="61b65-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="61b65-126">Modo perdido (solo iOS)</span><span class="sxs-lookup"><span data-stu-id="61b65-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="61b65-127">Buscar dispositivo (solo iOS)</span><span class="sxs-lookup"><span data-stu-id="61b65-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="61b65-128">Reiniciar (solo Windows)</span><span class="sxs-lookup"><span data-stu-id="61b65-128">Restart (Windows only)</span></span>

<span data-ttu-id="61b65-129">Para obtener más información sobre cada acción, consulte [Acciones de dispositivo disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="61b65-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>