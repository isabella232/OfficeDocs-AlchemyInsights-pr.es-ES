---
title: Administrador de extremos - Líneas de base de seguridad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51408798"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="d7f12-102">Administrador de extremos - Líneas de base de seguridad</span><span class="sxs-lookup"><span data-stu-id="d7f12-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="d7f12-103">Las líneas de base de seguridad son grupos preconfigurados de opciones de configuración de Windows que le ayudarán a aplicar las configuraciones de seguridad recomendadas por los equipos de seguridad correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d7f12-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="d7f12-104">Estas líneas de base se pueden personalizar para ofrecer solo la configuración y los valores deseados.</span><span class="sxs-lookup"><span data-stu-id="d7f12-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="d7f12-105">Para obtener más información acerca de las líneas base de seguridad, vea [Usar líneas de base de seguridad para configurar dispositivos con Windows 10 en Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="d7f12-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="d7f12-106">Actualmente hay líneas base para estos productos:</span><span class="sxs-lookup"><span data-stu-id="d7f12-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="d7f12-107">Configuración de seguridad de Windows MDM</span><span class="sxs-lookup"><span data-stu-id="d7f12-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="d7f12-108">Microsoft Defender para punto de conexión de seguridad</span><span class="sxs-lookup"><span data-stu-id="d7f12-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="d7f12-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d7f12-109">Microsoft Edge</span></span>

<span data-ttu-id="d7f12-110">Cada una de las líneas de base se actualiza periódicamente y se libera en versiones incrementales.</span><span class="sxs-lookup"><span data-stu-id="d7f12-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="d7f12-111">Cada versión agrega y quita la configuración de la versión anterior para asegurarse de que la línea de base cumple las instrucciones actuales.</span><span class="sxs-lookup"><span data-stu-id="d7f12-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="d7f12-112">La consola de líneas de base de seguridad en punto de conexión de seguridad permite comparar diferentes versiones haciendo visibles los cambios de una versión a otra.</span><span class="sxs-lookup"><span data-stu-id="d7f12-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="d7f12-113">Para obtener instrucciones sobre cómo cambiar de manera más eficaz la versión de línea de base que se implementa, vea [Administrar perfiles de línea de base de seguridad en Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="d7f12-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="d7f12-114">Después de implementar una línea base de seguridad, puede supervisar el estado de implementación y revisar la configuración en cada dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7f12-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="d7f12-115">**Nota:** Los datos de informes para líneas de base pueden tardar hasta 24 horas en aparecer desde la implementación inicial a un dispositivo y hasta 6 horas para obtener más actualizaciones.</span><span class="sxs-lookup"><span data-stu-id="d7f12-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="d7f12-116">La causa más común de que no se aplique una configuración de línea de base es porque la misma configuración se usa en un perfil diferente.</span><span class="sxs-lookup"><span data-stu-id="d7f12-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="d7f12-117">Para investigar este escenario para un dispositivo específico, seleccione ese dispositivo desde el nodo Estado del dispositivo del perfil de Línea de base de seguridad.</span><span class="sxs-lookup"><span data-stu-id="d7f12-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="d7f12-118">Para ver los detalles, consulte [Resolver conflictos de líneas de base de seguridad](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="d7f12-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>