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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702920"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="8a0ba-102">Supervisión del acceso condicional para Exchange</span><span class="sxs-lookup"><span data-stu-id="8a0ba-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="8a0ba-103">Los usuarios con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="8a0ba-104">Para solucionarlo, recomendamos una o varias de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="8a0ba-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="8a0ba-105">Si se supone que el dispositivo está inscrito, aconseje al usuario que vaya a la aplicación portal de empresa y compruebe que aparece en el portal de empresa.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="8a0ba-106">Si no lo hace, el usuario debería inscribir el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="8a0ba-107">En el portal de Azure, vaya a **Intune \> Compliance Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="8a0ba-108">En **supervisión** , haga clic en **cumplimiento del dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="8a0ba-109">Vea el informe de cumplimiento de dispositivos para comprobar que el dispositivo del usuario está marcado como compatible.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="8a0ba-110">En el portal de Azure, vaya a **Intune \> Compliance Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="8a0ba-111">En **administrar**, haga clic en **directivas**.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="8a0ba-112">En la lista de directivas de cumplimiento, compruebe que haya un perfil asignado al dispositivo del usuario.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="8a0ba-113">Si no hay ningún perfil asignado, Intune no podrá confirmar el estado de cumplimiento del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="8a0ba-114">Edite la asignación de acceso condicional del usuario.</span><span class="sxs-lookup"><span data-stu-id="8a0ba-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="8a0ba-115">En el portal de Azure, vaya a **Intune \> \> policies de acceso condicional**</span><span class="sxs-lookup"><span data-stu-id="8a0ba-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="8a0ba-116">Seleccionar una directiva de la lista</span><span class="sxs-lookup"><span data-stu-id="8a0ba-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="8a0ba-117">Haga clic en **usuarios y grupos**</span><span class="sxs-lookup"><span data-stu-id="8a0ba-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="8a0ba-118">Para dirigir una determinada Directiva a una persona, agréguela a la lista **incluir** .</span><span class="sxs-lookup"><span data-stu-id="8a0ba-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="8a0ba-119">Para asegurarse de que se omite una persona de la Directiva, agréguela a la lista de **exclusión** .</span><span class="sxs-lookup"><span data-stu-id="8a0ba-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="8a0ba-120">Más información: [cómo supervisar los dispositivos de acceso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="8a0ba-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

