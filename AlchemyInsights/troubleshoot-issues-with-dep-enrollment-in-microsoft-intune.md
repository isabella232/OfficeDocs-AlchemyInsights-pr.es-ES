---
title: Solucionar problemas con la inscripción de DEP en Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: e77295f0395919a723dcec1a313ca03154ae59b1bea22bf791f3a0f923cab60d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008275"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Solucionar problemas con la inscripción de DEP en Microsoft Intune

Revise los recursos que se enumeran a continuación para resolver el problema ahora.
  
1. Si el dispositivo DEP no puede inscribirse y mfa (autenticación multifactor) está habilitado, deshabilite MFA. Actualmente, MFA no es compatible con la inscripción de DEP

2. Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción. Revise [este documento para](https://docs.microsoft.com/intune/help-desk-operators) obtener más detalles.

3. Revise estos documentos para obtener una lista de errores comunes que impiden la inscripción y las resoluciones a cada uno: [Guía](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) de solución de problemas y documento de solución [de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

4. [Obtenga información sobre el programa de inscripción de dispositivos](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
