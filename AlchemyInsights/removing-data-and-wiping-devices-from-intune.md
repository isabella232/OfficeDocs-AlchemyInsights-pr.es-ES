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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701300"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="cf3e0-102">Eliminación de datos y borrado de dispositivos desde Intune</span><span class="sxs-lookup"><span data-stu-id="cf3e0-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="cf3e0-103">Las acciones remotas de eliminación y borrado de dispositivos se pueden usar para eliminar los datos de una empresa administrados por Intune, o para realizar un restablecimiento de fábrica y regresar al dispositivo a su configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="cf3e0-104">Inicie sesión en Administración de dispositivos de Microsoft 365 y diríjase a **Dispositivos** > **Todos los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="cf3e0-105">Seleccione el dispositivo que desea quitar.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="cf3e0-106">Seleccione el tipo de eliminación remota que desea realizar.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="cf3e0-107">La acción Eliminación solo borra la información de la organización, mientras que el borrado completo restaura el dispositivo a su configuración de fábrica.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="cf3e0-108">Seleccione **Sí** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="cf3e0-109">Hasta que la eliminación finalice, el estado de la acción del dispositivo se mostrará como Eliminación pendiente.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="cf3e0-110">Cuando se complete la acción, ya no verá el dispositivo móvil en la lista de dispositivos administrados.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="cf3e0-111">**Nota** Los datos de la empresa no se pueden eliminar de los dispositivos CONECTADOS a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cf3e0-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="cf3e0-112">Para obtener información detallada sobre el efecto de las acciones de eliminación y borrado, incluido lo que se conserva y lo que se elimina, consulte [Eliminar dispositivos con la función borrado, eliminación, o anular la inscripción en el dispositivo de forma manual](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="cf3e0-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="cf3e0-113">Para borrar todos los datos de un dispositivo macOS, consulte [Borrar todos los datos de un dispositivo macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="cf3e0-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>