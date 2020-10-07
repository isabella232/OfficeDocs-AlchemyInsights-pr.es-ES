---
title: Supervisión del acceso condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366445"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Supervisión del acceso condicional para Exchange

Los usuarios con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización. Para solucionarlo, recomendamos una o varias de las siguientes soluciones:

- Si se supone que el dispositivo está inscrito, aconseje al usuario que vaya a la aplicación portal de empresa y compruebe que aparece en el portal de empresa. Si no lo hace, el usuario debería inscribir el dispositivo.
- En el portal de Azure, vaya a Intune > el cumplimiento de dispositivos. En supervisión, haga clic en cumplimiento del dispositivo. Vea el informe de cumplimiento de dispositivos para comprobar que el dispositivo del usuario está marcado como compatible.
- En el portal de Azure, vaya a Intune > el cumplimiento de dispositivos. En administrar, haga clic en directivas. En la lista de directivas de cumplimiento, compruebe que haya un perfil asignado al dispositivo del usuario. Si no hay ningún perfil asignado, Intune no podrá confirmar el estado de cumplimiento del dispositivo.
- Edite la asignación de acceso condicional del usuario.

1. En el portal de Azure, vaya a **Intune**  >  **Conditional access**  >  **Policies**de acceso condicional.
2. Seleccione una directiva de la lista.
3. Haga clic en usuarios y grupos.
4. Para dirigir una determinada Directiva a una persona, agréguela a la lista incluir. Para asegurarse de que se omite una persona de la Directiva, agréguela a la lista de exclusión.

Vínculos útiles:

[Introducción al cumplimiento de dispositivos](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solución de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Directiva de solución de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Supervisión del cumplimiento de dispositivos de Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: estos pasos solo son útiles en la solución de problemas de acceso condicional a la característica de Azure Active Directory. También es posible poner en cuarentena un dispositivo que impida el acceso al correo electrónico con la Directiva de Exchange. Puede encontrar más información sobre la administración de dispositivos de Exchange [aquí](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
