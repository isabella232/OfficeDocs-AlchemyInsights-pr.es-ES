---
title: Directiva de protección de aplicaciones
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266467"
---
# <a name="application-protection-policy"></a><span data-ttu-id="43413-102">Directiva de protección de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="43413-102">Application protection policy</span></span>

<span data-ttu-id="43413-103">Si no está familiarizado con la Directiva de protección de aplicaciones (APP), consulte la [Introducción a las directivas de protección de aplicaciones](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="43413-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="43413-104">Para comenzar a usar la APP, consulte [Creación y asignación de directivas de protección de aplicaciones](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="43413-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="43413-105">Requisitos de la directiva de protección de aplicaciones:</span><span class="sxs-lookup"><span data-stu-id="43413-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="43413-106">El usuario tiene una licencia de Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="43413-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="43413-107">El usuario pertenece a un grupo al que se dirigen las directivas de protección de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="43413-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="43413-108">Solo un usuario corporativo ha iniciado sesión en aplicaciones protegidas en un dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43413-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="43413-109">La aplicación ha implementado el [SDK de Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="43413-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="43413-110">Para obtener una lista de las aplicaciones compatibles con el SDK, consulte [Aplicaciones protegidas de Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="43413-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="43413-111">Las directivas se aplican después de que un usuario que cumpla los requisitos anteriores inicie sesión en una aplicación compatible con el SDK de Intune.</span><span class="sxs-lookup"><span data-stu-id="43413-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="43413-112">La forma más sencilla de determinar si se aplica una directiva consiste en exigir que el usuario establezca un pin en la directiva.</span><span class="sxs-lookup"><span data-stu-id="43413-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="43413-113">Para obtener más información, vea:</span><span class="sxs-lookup"><span data-stu-id="43413-113">For more information, see:</span></span>

[<span data-ttu-id="43413-114">Preguntas más frecuentes sobre la solución de problemas de APP/MAM</span><span class="sxs-lookup"><span data-stu-id="43413-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="43413-115">Cómo validar la configuración de la Directiva de protección de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="43413-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="43413-116">Entender el tiempo de entrega de la Directiva de protección de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="43413-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="43413-117">Cómo supervisar directivas de protección de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="43413-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)