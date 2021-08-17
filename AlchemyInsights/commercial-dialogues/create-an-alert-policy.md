---
title: Crear una directiva de alerta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200002"
- "7670"
ms.openlocfilehash: 057a0c587c2bee69f94e1e35192145b013e901b9fa1831fccf566e7e64de5261
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894516"
---
# <a name="create-an-alert-policy"></a>Crear una directiva de alerta

1. En el Centro de cumplimiento de Microsoft 365 <https://security.microsoft.com> en , vaya a **Directivas** directivas de \> **alerta en** la **sección** Alerta.

   Para ir directamente a la **página Directiva de** alerta, use <https://compliance.microsoft.com/alertpolicies> .

2. Haga clic **en + Nueva directiva de alerta**.
3. En el menú desplegable del Asistente para directivas que aparece, continúe con la siguiente configuración:
   - **Asigne un nombre a** la página de alerta: escriba los valores **Name**, **Description** (optional), **Severity** y **Category** según corresponda a sus necesidades. Cuando termine, haga clic en **Siguiente**.
   - **Crear configuración de** alerta:  seleccione una actividad en el menú desplegable Actividad es y cualquier configuración adicional que aparezca, y seleccione las frecuencias de activación de alertas que satisfagan sus necesidades. Cuando termine, haga clic en **Siguiente**.

     > [!NOTE]
     > Solo puede elegir una actividad, pero puede agregar condiciones para refinar lo que detecta la directiva.

   - **Establecer la página** de destinatarios: decida si desea notificar a  los usuarios cuando se desencadene esta alerta seleccionando Enviar notificaciones por correo electrónico y eligiendo los destinatarios de correo electrónico **adecuados** y un límite de notificación **diario.** Cuando termine, haga clic en **Siguiente**.
   - **Revise la página de configuración:** Revise la configuración. Puede modificar la configuración haciendo clic en **Editar** en la sección correspondiente. Puedes activar la directiva de inmediato seleccionando **Sí, activala inmediatamente.**

   Cuando haya terminado, haga clic en **Finalizar**.

Para obtener más información, vea [Directivas de alerta en Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).
