---
title: Ejemplo de directiva de datos adjuntos seguros de Microsoft Defender para Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737572"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Ejemplo de directiva de datos adjuntos seguros de Microsoft Defender para Office 365

Estas opciones de configuración habilitan una directiva denominada *Sin* retrasos que entrega mensajes inmediatamente y, a continuación, vuelve a adjuntar datos adjuntos después de examinarse:

- **Nombre:** sin retrasos
- **Descripción:** entrega los mensajes inmediatamente y vuelve a adjuntar los datos adjuntos después del examen.
- **Respuesta:** seleccione la **opción Entrega** dinámica. Para obtener más información, vea [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Sección** Redirigir datos adjuntos: seleccione la opción Habilitar redireccionamiento **y,** a continuación, escriba la dirección de correo electrónico de su administrador global de Microsoft 365, administrador de seguridad o analista de seguridad que investigará datos adjuntos malintencionados.
- **Sección Aplicado a:** Seleccione **El dominio de destinatario es** y, a continuación, seleccione su dominio. Seleccione **agregar** y, a continuación, **seleccione Aceptar**. Una vez que haya terminado, seleccione **Guardar**.

Para obtener más información, vea [Datos adjuntos seguros en Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
