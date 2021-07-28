---
title: Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: aa89cbd58875f418a0a7a9db4b5eb4f0e4c1223a
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603293"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge

Microsoft Edge tiene problemas conocidos relacionados con las zonas de seguridad que pueden afectar el modo en que los usuarios de Azure inician sesión en Windows Admin Center. Para obtener más información, vea los [Problemas conocidos en Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Si tiene problemas para usar las características de Azure con Microsoft Edge, pruebe lo siguiente:

1. En el menú Inicio, en la barra **Buscar**, escriba **Opciones de Internet** y selecciónela.
1. En **Propiedades de Internet**, seleccione la pestaña **Seguridad**.
1. Seleccione **Sitios de confianza** y después **Sitios**.
1. Agregue la dirección URL de la puerta de enlace, así como <https://login.microsoftonline.com> y <https://login.live.com>, y seleccione **Cerrar**.
1. En **Propiedades de Internet**, seleccione la pestaña **Privacidad**.
1. En la sección Bloqueador de elementos emergentes, seleccione **Configuración**. Agregue la dirección URL de la puerta de enlace, así como <https://login.microsoftonline.com> y <https://login.live.com>, y después, seleccione **Cerrar**.