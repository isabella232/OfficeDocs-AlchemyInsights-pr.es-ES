---
title: Iniciar sesión en Microsoft Edge manualmente
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398674"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="27c9d-102">Iniciar sesión en Microsoft Edge manualmente</span><span class="sxs-lookup"><span data-stu-id="27c9d-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="27c9d-103">Si un usuario no ha iniciado sesión automáticamente durante una experiencia de primera ejecución, el usuario puede iniciar sesión manualmente a través de la configuración del explorador o el control de identidad.</span><span class="sxs-lookup"><span data-stu-id="27c9d-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="27c9d-104">Para administrar el inicio de sesión, use las siguientes directivas:</span><span class="sxs-lookup"><span data-stu-id="27c9d-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="27c9d-105">[NonRemovableProfileEnabled:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) para asegurarse de que un usuario siempre tiene un perfil de trabajo en Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="27c9d-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="27c9d-106">[RestrictSigninToPattern:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) para restringir el inicio de sesión a un conjunto de cuentas de confianza.</span><span class="sxs-lookup"><span data-stu-id="27c9d-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="27c9d-107">[BrowserSignin:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) para deshabilitar el inicio de sesión o para forzar a los usuarios a iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="27c9d-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

