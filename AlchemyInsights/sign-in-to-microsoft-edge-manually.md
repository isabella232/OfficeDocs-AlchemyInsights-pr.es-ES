---
title: Inicie sesión para Microsoft Edge manualmente
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
ms.openlocfilehash: f9aa27a585d805360e1fadecfd0db3b11d15a3594ed5bd5dc6c68cec37a4d6a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050783"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Inicie sesión para Microsoft Edge manualmente

Si un usuario no ha iniciado sesión automáticamente durante una experiencia de primera ejecución, el usuario puede iniciar sesión manualmente a través de la configuración del explorador o el control de identidad. Para administrar el inicio de sesión, use las siguientes directivas:

1. [NonRemovableProfileEnabled:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) para asegurarse de que un usuario siempre tiene un perfil de trabajo en Microsoft Edge.
2. [RestrictSigninToPattern:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) para restringir el inicio de sesión a un conjunto de cuentas de confianza.
3. [BrowserSignin:](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) para deshabilitar el inicio de sesión o para forzar a los usuarios a iniciar sesión.

