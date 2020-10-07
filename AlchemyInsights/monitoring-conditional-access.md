---
title: Supervisión del acceso condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366445"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="2627b-102">Supervisión del acceso condicional para Exchange</span><span class="sxs-lookup"><span data-stu-id="2627b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="2627b-103">Los usuarios con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización.</span><span class="sxs-lookup"><span data-stu-id="2627b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2627b-104">Para solucionarlo, recomendamos una o varias de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="2627b-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="2627b-105">Si se supone que el dispositivo está inscrito, aconseje al usuario que vaya a la aplicación portal de empresa y compruebe que aparece en el portal de empresa.</span><span class="sxs-lookup"><span data-stu-id="2627b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2627b-106">Si no lo hace, el usuario debería inscribir el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2627b-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="2627b-107">En el portal de Azure, vaya a Intune > el cumplimiento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2627b-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="2627b-108">En supervisión, haga clic en cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2627b-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="2627b-109">Vea el informe de cumplimiento de dispositivos para comprobar que el dispositivo del usuario está marcado como compatible.</span><span class="sxs-lookup"><span data-stu-id="2627b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="2627b-110">En el portal de Azure, vaya a Intune > el cumplimiento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2627b-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="2627b-111">En administrar, haga clic en directivas.</span><span class="sxs-lookup"><span data-stu-id="2627b-111">Under Manage, click Policies.</span></span> <span data-ttu-id="2627b-112">En la lista de directivas de cumplimiento, compruebe que haya un perfil asignado al dispositivo del usuario.</span><span class="sxs-lookup"><span data-stu-id="2627b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2627b-113">Si no hay ningún perfil asignado, Intune no podrá confirmar el estado de cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2627b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="2627b-114">Edite la asignación de acceso condicional del usuario.</span><span class="sxs-lookup"><span data-stu-id="2627b-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="2627b-115">En el portal de Azure, vaya a **Intune**  >  **Conditional access**  >  **Policies**de acceso condicional.</span><span class="sxs-lookup"><span data-stu-id="2627b-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="2627b-116">Seleccione una directiva de la lista.</span><span class="sxs-lookup"><span data-stu-id="2627b-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="2627b-117">Haga clic en usuarios y grupos.</span><span class="sxs-lookup"><span data-stu-id="2627b-117">Click Users and groups.</span></span>
4. <span data-ttu-id="2627b-118">Para dirigir una determinada Directiva a una persona, agréguela a la lista incluir.</span><span class="sxs-lookup"><span data-stu-id="2627b-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="2627b-119">Para asegurarse de que se omite una persona de la Directiva, agréguela a la lista de exclusión.</span><span class="sxs-lookup"><span data-stu-id="2627b-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="2627b-120">Vínculos útiles:</span><span class="sxs-lookup"><span data-stu-id="2627b-120">Helpful links:</span></span>

[<span data-ttu-id="2627b-121">Introducción al cumplimiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="2627b-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="2627b-122">Solución de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="2627b-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="2627b-123">Directiva de solución de problemas</span><span class="sxs-lookup"><span data-stu-id="2627b-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="2627b-124">Supervisión del cumplimiento de dispositivos de Intune</span><span class="sxs-lookup"><span data-stu-id="2627b-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="2627b-125">Nota: estos pasos solo son útiles en la solución de problemas de acceso condicional a la característica de Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2627b-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="2627b-126">También es posible poner en cuarentena un dispositivo que impida el acceso al correo electrónico con la Directiva de Exchange.</span><span class="sxs-lookup"><span data-stu-id="2627b-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="2627b-127">Puede encontrar más información sobre la administración de dispositivos de Exchange [aquí](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="2627b-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
