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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013765"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Errores de sincronización de inscripción automática de dispositivos de Apple

"Hemos detectado que tiene uno o varios tokens ADE/DEP que están en estado de error. Hasta que se resuelva el estado de error para cada token afectado, la funcionalidad de ADE no funcionará como se esperaba".

Este error puede manifestarse de varias maneras, como:

1. Es posible que los dispositivos no se sincronicen de ABM/ASM a Intune
2. Las asignaciones de perfiles de inscripción pueden estar fallando
3. Es posible que los dispositivos no completen la inscripción de ADE correctamente

Compruebe el error de sincronización notificado en la consola de Intune en **Dispositivos > Inscribir** dispositivos > la inscripción de Apple > tokens del programa de inscripción .

Una de las causas más comunes de error de sincronización es la expiración del token actual. En muchos casos, la renovación del token afectado resolverá el problema.

Si uno o varios de los tokens han expirado, consulte la siguiente documentación para ayudarle a renovarlos según corresponda:

[Renovar un token de inscripción automatizada de dispositivos](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Además, puede ver la siguiente documentación para ver posibles correcciones para otros errores que causan errores de sincronización de tokens:

[Errores de sincronización ABM/ASM para tokens de inscripción de dispositivos automatizados de iOS/iPadOS y macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Errores de sincronización ABM/ASM para tokens de inscripción de dispositivos automatizados de iOS/iPadOS y macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
