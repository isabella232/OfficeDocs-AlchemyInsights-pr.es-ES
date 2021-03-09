---
title: Uso del acceso condicional con Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529365"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="c70b5-102">Uso del acceso condicional con Intune</span><span class="sxs-lookup"><span data-stu-id="c70b5-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="c70b5-103">El uso del acceso condicional con Intune requiere 3 pasos:</span><span class="sxs-lookup"><span data-stu-id="c70b5-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="c70b5-104">Crea una directiva de cumplimiento para definir la configuración que debe cumplirse antes de que el dispositivo se considere compatible. Por ejemplo, un dispositivo debe tener una patilla de al menos 6 dígitos antes de considerarlo compatible.</span><span class="sxs-lookup"><span data-stu-id="c70b5-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="c70b5-105">Cree una directiva de acceso condicional que defina qué recursos se protegen y qué condiciones deben cumplirse para tener acceso a esos recursos. Por ejemplo, un dispositivo debe ser compatible antes de acceder al correo electrónico corporativo.</span><span class="sxs-lookup"><span data-stu-id="c70b5-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="c70b5-106">Asegúrese de que tanto las directivas de cumplimiento como las directivas de acceso condicional están dirigidas a los grupos de usuarios deseados. Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c70b5-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c70b5-107">Más información...</span><span class="sxs-lookup"><span data-stu-id="c70b5-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
