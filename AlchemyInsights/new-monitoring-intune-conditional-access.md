---
title: Supervisar el acceso condicional de Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327574"
---
# <a name="monitor-intune-conditional-access"></a>Supervisar el acceso condicional de Intune

Los usuarios dirigidos con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización. Para resolver, recomendamos una o varias de las siguientes soluciones:

1. Si se supone que el dispositivo está inscrito, aconseja al usuario que vaya a la aplicación Portal de empresa y compruebe que aparece en el Portal de empresa. Si no lo hace, el usuario debe inscribir el dispositivo.
1. En Azure Portal, vaya a Cumplimiento de   >  **dispositivos de** Intune. 
1. Para ver el informe de cumplimiento del dispositivo para comprobar que el dispositivo del usuario está marcado como compatible, en **Monitor**, haga clic en **Cumplimiento del dispositivo**.
1. En Azure Portal, vaya a Cumplimiento de   >  **dispositivos de** Intune. En **Administrar, haga** clic en **Directivas**. En la lista de directivas de cumplimiento, compruebe que un perfil está asignado al dispositivo del usuario. Si no se asigna ningún perfil, Intune no podrá confirmar el estado de cumplimiento del dispositivo.
1. Edite la asignación de acceso condicional del usuario.
1. En Azure Portal, vaya a Directivas de acceso condicional de **Intune,** seleccione una directiva de la lista y  >    >  haga clic **en Usuarios y grupos.**
1. Para dirigir una determinada directiva a alguien, agrégrela a la **lista Incluir**. Para asegurarse de que una persona se omite de la directiva, agrégrela a la **lista Excluir**.

**Vínculos útiles:**

- [Introducción al cumplimiento de dispositivos](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Solución de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Directiva de solución de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Supervisión del cumplimiento de dispositivos de Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Nota:** Estos pasos solo son útiles para solucionar problemas de la Azure Active Directory de acceso condicional. También es posible poner en cuarentena un dispositivo que bloquea su acceso al correo electrónico con Exchange directiva. Encontrará más información Exchange administración de [**dispositivos**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))aquí.
