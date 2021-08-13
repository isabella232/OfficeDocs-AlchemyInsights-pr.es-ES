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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975118"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Supervisión del acceso condicional para Exchange

Los usuarios dirigidos con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización. Para resolver, recomendamos una o varias de las siguientes soluciones:

- Si se supone que el dispositivo está inscrito, aconseja al usuario que vaya a la aplicación Portal de empresa y compruebe que aparece en el Portal de empresa. Si no lo hace, el usuario debe inscribir el dispositivo.
- En Azure Portal, vaya a Intune > cumplimiento de dispositivos. En Supervisar, haga clic en Cumplimiento del dispositivo. Consulta el informe de cumplimiento del dispositivo para comprobar que el dispositivo del usuario está marcado como compatible.
- En Azure Portal, vaya a Intune > cumplimiento de dispositivos. En Administrar, haga clic en Directivas. En la lista de directivas de cumplimiento, compruebe que un perfil está asignado al dispositivo del usuario. Si no se asigna ningún perfil, Intune no podrá confirmar el estado de cumplimiento del dispositivo.
- Edite la asignación de acceso condicional del usuario.

1. En Azure Portal, vaya a **Directivas**  >  **de acceso condicional de**  >  Intune.
2. Seleccione una directiva de la lista.
3. Haga clic en Usuarios y grupos.
4. Para dirigir una determinada directiva a alguien, agréguila a la lista Incluir. Para asegurarse de que una persona se omite de la directiva, agrégrela a la lista Excluir.

Vínculos útiles:

[Introducción al cumplimiento de dispositivos](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solución de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Directiva de solución de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Supervisión del cumplimiento de dispositivos de Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: estos pasos solo son útiles para solucionar problemas de la Azure Active Directory acceso condicional de la característica. También es posible poner en cuarentena un dispositivo que bloquea su acceso al correo electrónico con Exchange directiva. Encontrará más información Exchange administración de dispositivos [aquí]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
