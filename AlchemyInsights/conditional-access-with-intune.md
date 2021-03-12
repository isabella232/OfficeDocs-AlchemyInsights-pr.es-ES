---
title: Acceso condicional con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704803"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="7b1ce-102">Acceso condicional con Intune</span><span class="sxs-lookup"><span data-stu-id="7b1ce-102">Conditional Access with Intune</span></span>

<span data-ttu-id="7b1ce-103">El  **uso del acceso condicional**  con Intune requiere 3 pasos:</span><span class="sxs-lookup"><span data-stu-id="7b1ce-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="7b1ce-104">Crea una  **directiva de cumplimiento**  ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir la configuración que debe cumplirse antes de que el dispositivo se considere compatible.</span><span class="sxs-lookup"><span data-stu-id="7b1ce-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="7b1ce-105">Por ejemplo, un dispositivo debe tener una patilla de al menos 6 dígitos antes de considerarlo compatible.</span><span class="sxs-lookup"><span data-stu-id="7b1ce-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="7b1ce-106">Cree una **directiva de acceso condicional**  que defina qué recursos se protegen y qué condiciones deben cumplirse para tener acceso a esos recursos.</span><span class="sxs-lookup"><span data-stu-id="7b1ce-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="7b1ce-107">[Por ejemplo, un](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  dispositivo debe ser compatible antes de acceder al correo electrónico corporativo.</span><span class="sxs-lookup"><span data-stu-id="7b1ce-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="7b1ce-108">Asegúrese de **que tanto las directivas de cumplimiento**  como las  **directivas**  de acceso condicional están dirigidas a los grupos de usuarios deseados.</span><span class="sxs-lookup"><span data-stu-id="7b1ce-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="7b1ce-109">Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7b1ce-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="7b1ce-110">**Vínculos útiles:**</span><span class="sxs-lookup"><span data-stu-id="7b1ce-110">**Helpful links:**</span></span>

[<span data-ttu-id="7b1ce-111">Introducción al cumplimiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7b1ce-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="7b1ce-112">Solución de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="7b1ce-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7b1ce-113">Directiva de solución de problemas</span><span class="sxs-lookup"><span data-stu-id="7b1ce-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="7b1ce-114">Para proteger el correo electrónico (Exchange Online) del acceso por parte de dispositivos no conformes, se deben seguir ambos documentos:</span><span class="sxs-lookup"><span data-stu-id="7b1ce-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="7b1ce-115">Proteger el acceso de correo electrónico desde dispositivos con EAS</span><span class="sxs-lookup"><span data-stu-id="7b1ce-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="7b1ce-116">Proteger el acceso de correo electrónico desde dispositivos que usan clientes de autenticación modernos como Outlook</span><span class="sxs-lookup"><span data-stu-id="7b1ce-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)