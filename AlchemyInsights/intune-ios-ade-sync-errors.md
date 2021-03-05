---
title: Errores de sincronización de inscripción automática de dispositivos de Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448939"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="50e73-102">Errores de sincronización de inscripción automática de dispositivos de Apple</span><span class="sxs-lookup"><span data-stu-id="50e73-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="50e73-103">"Hemos detectado que tiene uno o varios tokens ADE/DEP que están en estado de error.</span><span class="sxs-lookup"><span data-stu-id="50e73-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="50e73-104">Hasta que se resuelva el estado de error para cada token afectado, la funcionalidad de ADE no funcionará como se esperaba".</span><span class="sxs-lookup"><span data-stu-id="50e73-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="50e73-105">Este error puede manifestarse de varias maneras, como:</span><span class="sxs-lookup"><span data-stu-id="50e73-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="50e73-106">Es posible que los dispositivos no se sincronicen de ABM/ASM a Intune</span><span class="sxs-lookup"><span data-stu-id="50e73-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="50e73-107">Las asignaciones de perfiles de inscripción pueden estar fallando</span><span class="sxs-lookup"><span data-stu-id="50e73-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="50e73-108">Es posible que los dispositivos no completen la inscripción de ADE correctamente</span><span class="sxs-lookup"><span data-stu-id="50e73-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="50e73-109">Compruebe el error de sincronización notificado en la consola de Intune en **Dispositivos > Inscribir** dispositivos > la inscripción de Apple > tokens del programa de inscripción .</span><span class="sxs-lookup"><span data-stu-id="50e73-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="50e73-110">Una de las causas más comunes de error de sincronización es la expiración del token actual.</span><span class="sxs-lookup"><span data-stu-id="50e73-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="50e73-111">En muchos casos, la renovación del token afectado resolverá el problema.</span><span class="sxs-lookup"><span data-stu-id="50e73-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="50e73-112">Si uno o varios de los tokens han expirado, consulte la siguiente documentación para ayudarle a renovarlos según corresponda:</span><span class="sxs-lookup"><span data-stu-id="50e73-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="50e73-113">Renovar un token de inscripción automatizada de dispositivos</span><span class="sxs-lookup"><span data-stu-id="50e73-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="50e73-114">Además, puede ver la siguiente documentación para ver posibles correcciones para otros errores que causan errores de sincronización de tokens:</span><span class="sxs-lookup"><span data-stu-id="50e73-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="50e73-115">Errores de sincronización ABM/ASM para tokens de inscripción de dispositivos automatizados de iOS/iPadOS y macOS</span><span class="sxs-lookup"><span data-stu-id="50e73-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="50e73-116">Errores de sincronización ABM/ASM para tokens de inscripción de dispositivos automatizados de iOS/iPadOS y macOS</span><span class="sxs-lookup"><span data-stu-id="50e73-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
