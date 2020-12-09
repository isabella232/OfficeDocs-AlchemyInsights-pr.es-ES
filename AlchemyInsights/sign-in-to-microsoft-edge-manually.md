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
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599509"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Iniciar sesión en Microsoft Edge manualmente

Si un usuario no inicia sesión automáticamente durante una experiencia de primera ejecución, el usuario puede iniciar sesión manualmente a través de la configuración del explorador o del control flotante de identidad. Para administrar el inicio de sesión, use las siguientes directivas:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) : para asegurarse de que un usuario siempre tiene un perfil de trabajo en Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) : para restringir el inicio de sesión a un conjunto de cuentas de confianza.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) : para deshabilitar el inicio de sesión o para obligar a los usuarios a iniciar sesión.

