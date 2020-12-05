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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576599"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge

Microsoft Edge tiene [problemas conocidos](https://go.microsoft.com/fwlink/?linkid=2140608) relacionados con las zonas de seguridad y pueden afectar al modo en que los usuarios de Azure inician sesión en el centro de administración de Windows. Si tienes problemas para usar las características de Azure con Microsoft Edge, prueba los siguientes pasos:

1. En el menú **Inicio** , busque **Opciones de Internet** y selecciónela.
2. En el cuadro de diálogo **propiedades de Internet** , vaya a la ficha **seguridad** .
3. Seleccione la zona **sitios de confianza** y, a continuación, seleccione el botón **sitios** .
4. En el cuadro de diálogo **sitios de confianza** , agregue la dirección URL de la puerta de enlace, así como [https://login.microsoftonline.com](https://login.microsoftonline.com) y y [https://login.live.com](https://login.live.com) , a continuación, seleccione **cerrar**.
5. En el cuadro de diálogo **propiedades de Internet** , vaya a la pestaña **privacidad** .
6. En la sección **bloqueador de ventanas emergentes** , seleccione **configuración**. En el cuadro de diálogo que se abre, agregue la dirección URL de la puerta de enlace, así como [https://login.microsoftonline.com](https://login.microsoftonline.com) y y [https://login.live.com](https://login.live.com) , a continuación, seleccione **cerrar**.
