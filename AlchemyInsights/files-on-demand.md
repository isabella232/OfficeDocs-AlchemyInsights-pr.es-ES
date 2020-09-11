---
title: Archivos a petición
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406612"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="7d439-102">Configurar Archivos a petición</span><span class="sxs-lookup"><span data-stu-id="7d439-102">Configure Files On-Demand</span></span>

<span data-ttu-id="7d439-103">Archivos a petición de OneDrive permite tener acceso a todos los archivos en OneDrive sin necesidad de descargarlos todos ni usar espacio de almacenamiento en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d439-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="7d439-104">Para configurar Archivos a petición en su PC:</span><span class="sxs-lookup"><span data-stu-id="7d439-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="7d439-105">Seleccione el icono de nube de color blanco o azul de **OneDrive** en el área de notificaciones de la barra de tareas de Windows.</span><span class="sxs-lookup"><span data-stu-id="7d439-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="7d439-106">Seleccione el icono de engranaje de **Ayuda y configuración** > **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="7d439-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="7d439-107">En la pestaña **Configuración**, seleccione la casilla **Ahorrar espacio y descargar archivos a medida que se usan**.</span><span class="sxs-lookup"><span data-stu-id="7d439-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="7d439-108">También puede configurar Archivos a petición con el registro.</span><span class="sxs-lookup"><span data-stu-id="7d439-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="7d439-109">Si usted deshabilita esta configuración, los usuarios de Windows 10 tienen el mismo comportamiento de sincronización que tienen los usuarios de versiones anteriores de Windows y no pueden activar los archivos a pedido.</span><span class="sxs-lookup"><span data-stu-id="7d439-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="7d439-110">Si no configura esta opción, los usuarios pueden activar o desactivar Archivos a petición.</span><span class="sxs-lookup"><span data-stu-id="7d439-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="7d439-111">Si habilita esta directiva, el valor de la siguiente clave del Registro se establece en “1”.</span><span class="sxs-lookup"><span data-stu-id="7d439-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="7d439-112">Si deshabilita esta directiva, el valor de la siguiente clave del registro se establece en 0.</span><span class="sxs-lookup"><span data-stu-id="7d439-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="7d439-113">Si no puede ver la opción de Archivos a petición en "Configuración", asegúrese de que el tipo de inicio del servicio "Controlador de filtro de archivos de la nube de Windows" está establecido en 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="7d439-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="7d439-114">Si habilita esta característica, el valor de la siguiente clave de registro se establece en 2.</span><span class="sxs-lookup"><span data-stu-id="7d439-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`