---
title: Supervisar el acceso condicional de Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417320"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="2718a-102">Supervisar el acceso condicional de Intune</span><span class="sxs-lookup"><span data-stu-id="2718a-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="2718a-103">Los usuarios dirigidos con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización.</span><span class="sxs-lookup"><span data-stu-id="2718a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2718a-104">Para resolver, recomendamos una o varias de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="2718a-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="2718a-105">Si se supone que el dispositivo está inscrito, aconseja al usuario que vaya a la aplicación Portal de empresa y compruebe que aparece en el Portal de empresa.</span><span class="sxs-lookup"><span data-stu-id="2718a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2718a-106">Si no lo hace, el usuario debe inscribir el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2718a-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="2718a-107">En Azure Portal, vaya a Cumplimiento de   >  **dispositivos de** Intune.</span><span class="sxs-lookup"><span data-stu-id="2718a-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="2718a-108">Para ver el informe de cumplimiento del dispositivo para comprobar que el dispositivo del usuario está marcado como compatible, en **Monitor**, haga clic en **Cumplimiento del dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="2718a-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="2718a-109">En Azure Portal, vaya a Cumplimiento de   >  **dispositivos de** Intune.</span><span class="sxs-lookup"><span data-stu-id="2718a-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="2718a-110">En **Administrar, haga** clic en **Directivas**.</span><span class="sxs-lookup"><span data-stu-id="2718a-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="2718a-111">En la lista de directivas de cumplimiento, compruebe que un perfil está asignado al dispositivo del usuario.</span><span class="sxs-lookup"><span data-stu-id="2718a-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2718a-112">Si no se asigna ningún perfil, Intune no podrá confirmar el estado de cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2718a-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="2718a-113">Edite la asignación de acceso condicional del usuario.</span><span class="sxs-lookup"><span data-stu-id="2718a-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="2718a-114">En Azure Portal, vaya a Directivas de acceso condicional de **Intune,** seleccione una directiva de la lista y  >    >  haga clic **en Usuarios y grupos.**</span><span class="sxs-lookup"><span data-stu-id="2718a-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="2718a-115">Para dirigir una determinada directiva a alguien, agrégrela a la **lista Incluir**.</span><span class="sxs-lookup"><span data-stu-id="2718a-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="2718a-116">Para asegurarse de que una persona se omite de la directiva, agrégrela a la **lista Excluir**.</span><span class="sxs-lookup"><span data-stu-id="2718a-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="2718a-117">**Vínculos útiles:**</span><span class="sxs-lookup"><span data-stu-id="2718a-117">**Helpful links:**</span></span>

- [<span data-ttu-id="2718a-118">Introducción al cumplimiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="2718a-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="2718a-119">Solución de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="2718a-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="2718a-120">Directiva de solución de problemas</span><span class="sxs-lookup"><span data-stu-id="2718a-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="2718a-121">Supervisión del cumplimiento de dispositivos de Intune</span><span class="sxs-lookup"><span data-stu-id="2718a-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="2718a-122">Estos pasos solo son útiles para solucionar problemas de la característica de Azure Active Directory Acceso condicional.</span><span class="sxs-lookup"><span data-stu-id="2718a-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="2718a-123">También es posible poner en cuarentena un dispositivo que bloquea su acceso al correo electrónico con la directiva de Exchange.</span><span class="sxs-lookup"><span data-stu-id="2718a-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="2718a-124">Encontrará más información sobre la administración de dispositivos exchange [**aquí**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="2718a-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
