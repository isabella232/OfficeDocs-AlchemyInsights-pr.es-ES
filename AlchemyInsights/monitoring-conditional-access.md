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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708691"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0d748-102">Supervisión del acceso condicional para Exchange</span><span class="sxs-lookup"><span data-stu-id="0d748-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0d748-103">Los usuarios dirigidos con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización.</span><span class="sxs-lookup"><span data-stu-id="0d748-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0d748-104">Para resolver, recomendamos una o varias de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="0d748-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="0d748-105">Si se supone que el dispositivo está inscrito, aconseja al usuario que vaya a la aplicación Portal de empresa y compruebe que aparece en el Portal de empresa.</span><span class="sxs-lookup"><span data-stu-id="0d748-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0d748-106">Si no lo hace, el usuario debe inscribir el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d748-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="0d748-107">En Azure Portal, vaya a Intune > cumplimiento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0d748-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0d748-108">En Supervisar, haga clic en Cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d748-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="0d748-109">Consulta el informe de cumplimiento del dispositivo para comprobar que el dispositivo del usuario está marcado como compatible.</span><span class="sxs-lookup"><span data-stu-id="0d748-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="0d748-110">En Azure Portal, vaya a Intune > cumplimiento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0d748-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0d748-111">En Administrar, haga clic en Directivas.</span><span class="sxs-lookup"><span data-stu-id="0d748-111">Under Manage, click Policies.</span></span> <span data-ttu-id="0d748-112">En la lista de directivas de cumplimiento, compruebe que un perfil está asignado al dispositivo del usuario.</span><span class="sxs-lookup"><span data-stu-id="0d748-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0d748-113">Si no se asigna ningún perfil, Intune no podrá confirmar el estado de cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d748-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="0d748-114">Edite la asignación de acceso condicional del usuario.</span><span class="sxs-lookup"><span data-stu-id="0d748-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="0d748-115">En Azure Portal, vaya a **Directivas**  >  **de acceso condicional de**  >  Intune.</span><span class="sxs-lookup"><span data-stu-id="0d748-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="0d748-116">Seleccione una directiva de la lista.</span><span class="sxs-lookup"><span data-stu-id="0d748-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="0d748-117">Haga clic en Usuarios y grupos.</span><span class="sxs-lookup"><span data-stu-id="0d748-117">Click Users and groups.</span></span>
4. <span data-ttu-id="0d748-118">Para dirigir una determinada directiva a alguien, agréguila a la lista Incluir.</span><span class="sxs-lookup"><span data-stu-id="0d748-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="0d748-119">Para asegurarse de que una persona se omite de la directiva, agrégrela a la lista Excluir.</span><span class="sxs-lookup"><span data-stu-id="0d748-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="0d748-120">Vínculos útiles:</span><span class="sxs-lookup"><span data-stu-id="0d748-120">Helpful links:</span></span>

[<span data-ttu-id="0d748-121">Introducción al cumplimiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="0d748-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="0d748-122">Solución de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="0d748-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0d748-123">Directiva de solución de problemas</span><span class="sxs-lookup"><span data-stu-id="0d748-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="0d748-124">Supervisión del cumplimiento de dispositivos de Intune</span><span class="sxs-lookup"><span data-stu-id="0d748-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="0d748-125">Nota: estos pasos solo son útiles para solucionar problemas de la característica de Azure Active Directory Acceso condicional.</span><span class="sxs-lookup"><span data-stu-id="0d748-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="0d748-126">También es posible poner en cuarentena un dispositivo que bloquea su acceso al correo electrónico con la directiva de Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d748-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="0d748-127">Encontrará más información sobre la administración de dispositivos exchange [aquí]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="0d748-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
