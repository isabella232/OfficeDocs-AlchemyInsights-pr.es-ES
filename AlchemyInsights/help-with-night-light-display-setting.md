---
title: Ayuda con la configuración de la pantalla de luz nocturna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123144"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="c983f-102">Ayuda con la configuración de la pantalla de luz nocturna</span><span class="sxs-lookup"><span data-stu-id="c983f-102">Help with the night light display setting</span></span>

<span data-ttu-id="c983f-103">Para obtener más información sobre la configuración de la pantalla de luz nocturna, vea [Configurar la pantalla de luz nocturna en Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="c983f-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="c983f-104">Si las opciones de luz nocturna están atenuadas en Configuración, compruebe la pantalla:</span><span class="sxs-lookup"><span data-stu-id="c983f-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="c983f-105">Haga clic en el cuadro de búsqueda de la barra de tareas y escriba **Administrador de dispositivos** y, después, seleccione **Administrador de dispositivos** de la lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="c983f-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="c983f-106">Expandir **Adaptadores de pantalla**.</span><span class="sxs-lookup"><span data-stu-id="c983f-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="c983f-107">Desafortunadamente, la característica de luz nocturna no está disponible si el dispositivo usa un controlador DisplayLink o un controlador de pantalla básico.</span><span class="sxs-lookup"><span data-stu-id="c983f-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="c983f-108">La característica de luz noctura usa tecnología de gráficos recientes, por lo que es posible que necesite actualizar el controlador de pantalla:</span><span class="sxs-lookup"><span data-stu-id="c983f-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="c983f-109">Busque actualizaciones en **Inicio** > **Configuración** > **Actualización y seguridad** > **Windows Update** > **Buscar actualizaciones**.</span><span class="sxs-lookup"><span data-stu-id="c983f-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="c983f-110">O</span><span class="sxs-lookup"><span data-stu-id="c983f-110">OR</span></span>

- <span data-ttu-id="c983f-111">Visite el sitio web de soporte técnico de su fabricante de hardware para descargar e instalar manualmente los controladores de visualización más recientes.</span><span class="sxs-lookup"><span data-stu-id="c983f-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="c983f-112">Restablecer la luz nocturna en el registro</span><span class="sxs-lookup"><span data-stu-id="c983f-112">Reset night light in the registry</span></span>

<span data-ttu-id="c983f-113">Si la actualización del controlador de pantalla no funciona, puede que necesite restablecer la luz nocturna en el registro.</span><span class="sxs-lookup"><span data-stu-id="c983f-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="c983f-114">**Precaución:** Este paso para solucionar problemas solo se recomienda para usuarios expertos.</span><span class="sxs-lookup"><span data-stu-id="c983f-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="c983f-115">La modificación incorrecta del registro puede producir graves problemas.</span><span class="sxs-lookup"><span data-stu-id="c983f-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="c983f-116">Para mayor protección, haga copia de seguridad del registro antes de modificarlo para poder restaurarlo si hay problemas.</span><span class="sxs-lookup"><span data-stu-id="c983f-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="c983f-117">En el cuadro de búsqueda, escriba **Regedit** y, después, seleccione **Editor del Registro** en los resultados de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="c983f-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="c983f-118">Vaya a la siguiente clave del registro:</span><span class="sxs-lookup"><span data-stu-id="c983f-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="c983f-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="c983f-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="c983f-120">Exporte y elimine la siguiente subclave:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="c983f-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="c983f-121">Exporte y elimine la siguiente subclave:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="c983f-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="c983f-122">Reinicie Windows y compruebe si las opciones de luz nocturna están disponibles.</span><span class="sxs-lookup"><span data-stu-id="c983f-122">Restart Windows and verify if the night light options are available.</span></span>


