---
title: Errores de sincronización de inscripción automática de dispositivos de Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707914"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="2bcdd-102">Errores de sincronización de inscripción automática de dispositivos de Apple</span><span class="sxs-lookup"><span data-stu-id="2bcdd-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="2bcdd-103">"Hemos detectado que tiene uno o varios tokens ADE/DEP que están en estado de error.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="2bcdd-104">Hasta que el estado del error se resuelva para cada token afectado, la funcionalidad de ADE no funcionará de la misma forma.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="2bcdd-105">Este error puede manifestarse de varias formas, entre las que se incluyen:</span><span class="sxs-lookup"><span data-stu-id="2bcdd-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="2bcdd-106">Es posible que los dispositivos no se sincronicen desde ABM/ASM a Intune</span><span class="sxs-lookup"><span data-stu-id="2bcdd-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="2bcdd-107">Es posible que se produzca un error en las asignaciones del perfil de inscripción</span><span class="sxs-lookup"><span data-stu-id="2bcdd-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="2bcdd-108">Es posible que los dispositivos no completen correctamente la inscripción ADE</span><span class="sxs-lookup"><span data-stu-id="2bcdd-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="2bcdd-109">Compruebe el error de sincronización que se indica en la consola de Intune en **dispositivos > inscribir dispositivos > los tokens del programa de inscripción >** inscripción de Apple y revise la siguiente documentación para ver cualquier posible corrección:</span><span class="sxs-lookup"><span data-stu-id="2bcdd-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="2bcdd-110">Errores de sincronización de ABM/ASM para iOS/iPados y tokens de inscripción de dispositivos automatizados para macOS</span><span class="sxs-lookup"><span data-stu-id="2bcdd-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
