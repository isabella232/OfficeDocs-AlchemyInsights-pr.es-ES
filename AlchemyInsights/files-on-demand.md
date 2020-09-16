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
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745305"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="f8b28-102">Configurar Archivos a petición</span><span class="sxs-lookup"><span data-stu-id="f8b28-102">Configure Files On-Demand</span></span>

<span data-ttu-id="f8b28-103">Archivos a petición de OneDrive permite tener acceso a todos los archivos en OneDrive sin necesidad de descargarlos todos ni usar espacio de almacenamiento en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8b28-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="f8b28-104">Para configurar Archivos a petición en su PC:</span><span class="sxs-lookup"><span data-stu-id="f8b28-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="f8b28-105">Seleccione el icono de nube de color blanco o azul de **OneDrive** en el área de notificaciones de la barra de tareas de Windows.</span><span class="sxs-lookup"><span data-stu-id="f8b28-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="f8b28-106">Seleccione el icono de engranaje de **Ayuda y configuración** > **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="f8b28-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="f8b28-107">En la pestaña **Configuración**, seleccione la casilla **Ahorrar espacio y descargar archivos a medida que se usan**.</span><span class="sxs-lookup"><span data-stu-id="f8b28-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="f8b28-108">También puede configurar Archivos a petición con el registro.</span><span class="sxs-lookup"><span data-stu-id="f8b28-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="f8b28-109">Si usted deshabilita esta configuración, los usuarios de Windows 10 tienen el mismo comportamiento de sincronización que tienen los usuarios de versiones anteriores de Windows y no pueden activar los archivos a pedido.</span><span class="sxs-lookup"><span data-stu-id="f8b28-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="f8b28-110">Si no configura esta opción, los usuarios pueden activar o desactivar Archivos a petición.</span><span class="sxs-lookup"><span data-stu-id="f8b28-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="f8b28-111">Si habilita esta directiva, el valor de la siguiente clave del Registro se establece en “1”.</span><span class="sxs-lookup"><span data-stu-id="f8b28-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="f8b28-112">Si deshabilita esta directiva, el valor de la siguiente clave del registro se establece en 0.</span><span class="sxs-lookup"><span data-stu-id="f8b28-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="f8b28-113">Si no puede ver la opción de Archivos a petición en "Configuración", asegúrese de que el tipo de inicio del servicio "Controlador de filtro de archivos de la nube de Windows" está establecido en 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="f8b28-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="f8b28-114">Si habilita esta característica, el valor de la siguiente clave de registro se establece en 2.</span><span class="sxs-lookup"><span data-stu-id="f8b28-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`