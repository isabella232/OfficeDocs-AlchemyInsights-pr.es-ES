---
title: Directiva de protección de aplicaciones
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969988"
---
# <a name="application-protection-policy"></a>Directiva de protección de aplicaciones

Si no está familiarizado con la Directiva de protección de aplicaciones (APP), consulte la [Introducción a las directivas de protección de aplicaciones](https://docs.microsoft.com/intune/apps/app-protection-policy).

Para comenzar a usar la APP, consulte [Creación y asignación de directivas de protección de aplicaciones](https://docs.microsoft.com/intune/app-protection-policies).

Requisitos de la directiva de protección de aplicaciones:

- El usuario tiene una licencia de Intune o EMS.
- El usuario pertenece a un grupo al que se dirigen las directivas de protección de aplicaciones.
- Solo un usuario corporativo ha iniciado sesión en aplicaciones protegidas en un dispositivo.
- La aplicación ha implementado el [SDK de Intune](https://docs.microsoft.com/intune/app-sdk-get-started). Para obtener una lista de las aplicaciones compatibles con el SDK, consulte [Aplicaciones protegidas de Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Las directivas se aplican después de que un usuario que cumpla los requisitos anteriores inicie sesión en una aplicación compatible con el SDK de Intune. La forma más sencilla de determinar si se aplica una directiva consiste en exigir que el usuario establezca un pin en la directiva. 

Para obtener más información, vea:

[Preguntas más frecuentes sobre la solución de problemas de APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Cómo validar la configuración de la Directiva de protección de aplicaciones](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Entender el tiempo de entrega de la Directiva de protección de aplicaciones](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Cómo supervisar directivas de protección de aplicaciones](https://docs.microsoft.com/intune/app-protection-policies-monitor)