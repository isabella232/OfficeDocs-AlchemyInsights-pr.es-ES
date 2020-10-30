---
title: Archivos a petición
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791311"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="7f469-102">Configurar Archivos a petición</span><span class="sxs-lookup"><span data-stu-id="7f469-102">Configure Files On-Demand</span></span>

<span data-ttu-id="7f469-103">Los archivos de OneDrive según demanda requieren[Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040)(versión 1709 o posterior) o Windows Server 2019 y OneDrive compilación 17.3.7064.1005 o posterior.</span><span class="sxs-lookup"><span data-stu-id="7f469-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="7f469-104">Archivos a petición de OneDrive permite tener acceso a todos los archivos en OneDrive sin necesidad de descargarlos todos ni usar espacio de almacenamiento en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f469-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="7f469-105">Para configurar Archivos a petición en su PC:</span><span class="sxs-lookup"><span data-stu-id="7f469-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="7f469-106">Seleccione el icono de nube de color blanco o azul de **OneDrive** en el área de notificaciones de la barra de tareas de Windows.</span><span class="sxs-lookup"><span data-stu-id="7f469-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="7f469-107">Seleccione el icono de engranaje de **Ayuda y configuración** > **Configuración** .</span><span class="sxs-lookup"><span data-stu-id="7f469-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="7f469-108">En la pestaña **Configuración** , seleccione la casilla **Ahorrar espacio y descargar archivos a medida que se usan** .</span><span class="sxs-lookup"><span data-stu-id="7f469-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="7f469-109">También puede configurar Archivos a petición con el registro.</span><span class="sxs-lookup"><span data-stu-id="7f469-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="7f469-110">Si usted deshabilita esta configuración, los usuarios de Windows 10 tienen el mismo comportamiento de sincronización que tienen los usuarios de versiones anteriores de Windows y no pueden activar los archivos a pedido.</span><span class="sxs-lookup"><span data-stu-id="7f469-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="7f469-111">Si no configura esta opción, los usuarios pueden activar o desactivar Archivos a petición.</span><span class="sxs-lookup"><span data-stu-id="7f469-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="7f469-112">Si habilita esta directiva, el valor de la siguiente clave del Registro se establece en “1”.</span><span class="sxs-lookup"><span data-stu-id="7f469-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="7f469-113">Si deshabilita esta directiva, el valor de la siguiente clave del registro se establece en 0.</span><span class="sxs-lookup"><span data-stu-id="7f469-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="7f469-114">Si no puede ver la opción de Archivos a petición en "Configuración", asegúrese de que el tipo de inicio del servicio "Controlador de filtro de archivos de la nube de Windows" está establecido en 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="7f469-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="7f469-115">Si habilita esta característica, el valor de la siguiente clave de registro se establece en 2.</span><span class="sxs-lookup"><span data-stu-id="7f469-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`