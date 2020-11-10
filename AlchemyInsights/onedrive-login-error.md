---
title: AADSTS50011 de error de inicio de sesión de OneDrive
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947533"
---
# <a name="onedrive-login-error-aadsts50011"></a>AADSTS50011 de error de inicio de sesión de OneDrive

Si recibe un error "AADSTS50011: la dirección URL de respuesta especificada en la solicitud no coincide con la respuesta" al iniciar sesión en la aplicación de OneDrive, compruebe lo siguiente:

La versión de OneDrive debe ser igual o mayor que la versión 20.052. XXXX. XXX. Para comprobar la versión, haga clic en el icono azul de OneDrive del área de notificación, seleccione **ayuda & configuración > configuración > acerca de**.

La red podría bloquear el tráfico a **g.Live.com** y **oneclient.SFX.ms**. Si se bloquea el tráfico, OneDrive no puede actualizarse a sí mismo. Trabaje con el administrador de la red para asegurarse de que tiene acceso a esas direcciones URL. [Estos extremos](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) deben ser accesibles para los clientes que usen planes de Microsoft 365.

Si necesita obtener manualmente una versión actual de OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
