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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Errores de sincronización de inscripción automática de dispositivos de Apple

"Hemos detectado que tiene uno o varios tokens ADE/DEP que están en estado de error. Hasta que el estado del error se resuelva para cada token afectado, la funcionalidad de ADE no funcionará de la misma forma.

Este error puede manifestarse de varias formas, entre las que se incluyen:

1. Es posible que los dispositivos no se sincronicen desde ABM/ASM a Intune
2. Es posible que se produzca un error en las asignaciones del perfil de inscripción
3. Es posible que los dispositivos no completen correctamente la inscripción ADE

Compruebe el error de sincronización que se indica en la consola de Intune en **dispositivos > inscribir dispositivos > los tokens del programa de inscripción >** inscripción de Apple y revise la siguiente documentación para ver cualquier posible corrección:

[Errores de sincronización de ABM/ASM para iOS/iPados y tokens de inscripción de dispositivos automatizados para macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
