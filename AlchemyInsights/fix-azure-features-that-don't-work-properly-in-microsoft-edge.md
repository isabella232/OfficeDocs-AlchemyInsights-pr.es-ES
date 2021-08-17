---
title: Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117105"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge

Microsoft Edge problemas [conocidos relacionados](https://go.microsoft.com/fwlink/?linkid=2140608) con las zonas de seguridad y pueden afectar a la forma en que los usuarios de Azure inician sesión en Windows Centro de administración. Si tiene problemas para usar las características de Azure Microsoft Edge, siga estos pasos:

1. En el **menú** Inicio, busque Opciones **de Internet** y selecciónelo.
2. En el cuadro de diálogo Propiedades de **Internet,** vaya a la **pestaña** Seguridad.
3. Seleccione la **zona Sitios de** confianza y, a continuación, seleccione el **botón** Sitios.
4. En el **cuadro de diálogo Sitios** de confianza, agregue la dirección URL de la puerta de enlace y, a continuación, seleccione [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) **Cerrar**.
5. En el cuadro de diálogo Propiedades de **Internet,** vaya a la **pestaña** Privacidad.
6. En la **sección Bloqueador de** elementos emergentes, **seleccione Configuración**. En el cuadro de diálogo que se abre, agregue la dirección URL de la puerta de enlace, así como [https://login.microsoftonline.com](https://login.microsoftonline.com) y [https://login.live.com](https://login.live.com) , y, a continuación, **seleccione Cerrar**.
