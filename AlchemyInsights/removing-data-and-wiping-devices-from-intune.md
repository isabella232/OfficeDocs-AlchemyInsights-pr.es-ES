---
title: Eliminación de datos y borrado de dispositivos desde Intune
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416330"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="9ffaf-102">Eliminación de datos y borrado de dispositivos desde Intune</span><span class="sxs-lookup"><span data-stu-id="9ffaf-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="9ffaf-103">Las acciones remotas de eliminación y borrado de dispositivos se pueden usar para eliminar los datos de una empresa administrados por Intune, o para realizar un restablecimiento de fábrica y regresar al dispositivo a su configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="9ffaf-104">Inicie sesión en Administración de dispositivos de Microsoft 365 y diríjase a **Dispositivos** > **Todos los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="9ffaf-105">Seleccione el dispositivo que desea quitar.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="9ffaf-106">Seleccione el tipo de eliminación remota que desea realizar.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="9ffaf-107">La acción Eliminación solo borra la información de la organización, mientras que el borrado completo restaura el dispositivo a su configuración de fábrica.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="9ffaf-108">Seleccione **Sí** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="9ffaf-109">Hasta que la eliminación finalice, el estado de la acción del dispositivo se mostrará como *Eliminación pendiente*.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="9ffaf-110">Cuando se haya completado esta acción, ya no verá el dispositivo móvil en la lista de dispositivos administrados.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="9ffaf-111">Los datos de la empresa no se pueden eliminar de los dispositivos CONECTADOS a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="9ffaf-112">Para obtener todos los detalles del efecto de las acciones Retirar y Borrar, incluido lo que se conserva y lo que se elimina, vea la documentación siguiente:</span><span class="sxs-lookup"><span data-stu-id="9ffaf-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="9ffaf-113">[Quite dispositivos mediante el borrado, retirada o desenrollando manualmente el](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="9ffaf-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="9ffaf-114">Cómo borrar solo los datos corporativos desde aplicaciones administradas por Intune</span><span class="sxs-lookup"><span data-stu-id="9ffaf-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="9ffaf-115">[Borrar todos los datos desde un dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="9ffaf-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>