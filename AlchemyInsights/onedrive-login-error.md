---
title: OneDrive error de inicio de sesión AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112929"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive error de inicio de sesión AADSTS50011

Si recibe un error "AADSTS50011: la dirección URL de respuesta especificada en la solicitud no coincide con la respuesta" al iniciar sesión en la aplicación OneDrive, compruebe lo siguiente:

La OneDrive debe ser igual o mayor que la versión 20.052.XXXX.XXXX. Para comprobar la versión, haga clic en el icono OneDrive en el área de notificación, seleccione **Ayuda & Configuración > Configuración > Acerca de**.

La red puede bloquear el tráfico **g.live.com** y **oneclient.sfx.ms**. Si ese tráfico está bloqueado, OneDrive no se puede actualizar. Trabaje con el administrador de red para asegurarse de que tiene acceso a esas direcciones URL. [Estos puntos de conexión](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) deben ser accesibles para los clientes que usan Microsoft 365 planes.

Si necesita obtener manualmente una versión actual de OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
