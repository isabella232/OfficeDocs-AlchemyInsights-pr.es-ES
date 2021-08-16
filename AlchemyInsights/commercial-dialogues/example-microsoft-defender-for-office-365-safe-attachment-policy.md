---
title: Ejemplo de Microsoft Defender para la directiva Office 365 Caja fuerte datos adjuntos
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988312"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Ejemplo de Microsoft Defender para la directiva Office 365 Caja fuerte datos adjuntos

Estas opciones de configuración habilitan una directiva denominada *Sin* retrasos que entrega mensajes inmediatamente y, a continuación, vuelve a adjuntar datos adjuntos después de examinarse:

- **Nombre:** sin retrasos
- **Descripción:** entrega los mensajes inmediatamente y vuelve a adjuntar los datos adjuntos después del examen.
- **Respuesta:** seleccione la **opción Entrega** dinámica. Para obtener más información, vea [Dynamic Delivery in Caja fuerte Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Sección Redirigir datos** adjuntos: seleccione la opción Habilitar redireccionamiento y escriba la dirección de correo electrónico de su Microsoft 365 administrador global, administrador de seguridad o analista de seguridad que investigará datos adjuntos malintencionados. 
- **Sección Aplicado a:** Seleccione **El dominio de destinatario es** y, a continuación, seleccione su dominio. Seleccione **agregar** y, a continuación, **seleccione Aceptar**. Una vez que haya terminado, seleccione **Guardar**.

Para obtener más información, [vea Caja fuerte attachments in Microsoft Defender para obtener Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
