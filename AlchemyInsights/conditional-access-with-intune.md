---
title: Acceso condicional con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931453"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="65626-102">Acceso condicional con Intune</span><span class="sxs-lookup"><span data-stu-id="65626-102">Conditional Access with Intune</span></span>

<span data-ttu-id="65626-103">El uso de **acceso condicional** con Intune requiere 3 pasos:</span><span class="sxs-lookup"><span data-stu-id="65626-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="65626-104">Cree una **Directiva de cumplimiento** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir la configuración que se debe cumplir antes de que el dispositivo se considere conforme.</span><span class="sxs-lookup"><span data-stu-id="65626-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="65626-105">Por ejemplo, un dispositivo debe tener un PIN de al menos 6 dígitos antes de que se considere compatible.</span><span class="sxs-lookup"><span data-stu-id="65626-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="65626-106">Cree una **Directiva de acceso condicional** que defina los recursos que se van a proteger y las condiciones que deben cumplirse para obtener acceso a esos recursos.</span><span class="sxs-lookup"><span data-stu-id="65626-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="65626-107">[Por ejemplo,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) un dispositivo debe ser compatible antes de obtener acceso al correo electrónico corporativo.</span><span class="sxs-lookup"><span data-stu-id="65626-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="65626-108">Asegúrese de que las directivas de **cumplimiento** y **las directivas de acceso condicional** estén dirigidas a los grupos de usuarios deseados.</span><span class="sxs-lookup"><span data-stu-id="65626-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="65626-109">Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65626-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="65626-110">**Vínculos útiles:**</span><span class="sxs-lookup"><span data-stu-id="65626-110">**Helpful links:**</span></span>

[<span data-ttu-id="65626-111">Introducción al cumplimiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="65626-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="65626-112">Solución de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="65626-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="65626-113">Directiva de solución de problemas</span><span class="sxs-lookup"><span data-stu-id="65626-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="65626-114">Para proteger el correo electrónico (Exchange Online) del acceso de dispositivos no compatibles, se deben seguir ambos documentos:</span><span class="sxs-lookup"><span data-stu-id="65626-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="65626-115">Proteger el acceso al correo electrónico de dispositivos con EAS</span><span class="sxs-lookup"><span data-stu-id="65626-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="65626-116">Proteger el acceso al correo electrónico desde dispositivos con clientes de autenticación modernos como Outlook</span><span class="sxs-lookup"><span data-stu-id="65626-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)