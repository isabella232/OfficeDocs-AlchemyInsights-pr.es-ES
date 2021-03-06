---
title: Cifrar automáticamente determinados mensajes de correo electrónico de office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510223"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Cifrar automáticamente determinados mensajes de correo electrónico de office 365

1. En el [Centro de administración de Exchange,](https://outlook.office365.com/ecp/)elija flujo de correo > **reglas**. 
2. Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar el cifrado de mensajes de Office **365** y la protección de derechos a los mensajes .
3. En **Nombre**, escriba un nombre para la regla, como *Cifrar todos los mensajes*.
4. En **Aplicar esta regla si**, elija **[Aplicar a todos los mensajes]**. 
5. Junto al campo **Hacer lo siguiente,** haga clic **en Seleccionar uno**. 
6. En el **menú desplegable Plantilla RMS,** seleccione **Cifrar** y, a continuación, haga clic en **Aceptar**. (Si no ve esta opción, significa que el plan no incluye cifrado automático. Pero puedes agregarlo!
7. Active la **casilla Auditar esta regla con** el nivel de gravedad y, a continuación, seleccione el nivel deseado. Si su empresa tiene obligaciones contractuales para enviar todos los correos electrónicos cifrados, le recomiendo establecer el nivel en **Alto**.
8. En **Elegir un modelo para esta regla,** haga clic en **Exigir**. 
9. Elija cualquier selección opcional (de una lista de selecciones opcionales que puede realizar en este momento, muchas de las cuales se pueden dejar con la configuración predeterminada para simplificar).
10. Haga clic en **Guardar**.

> [!IMPORTANT]
> Siempre puede volver y editar esta regla más adelante.

Para obtener más información sobre cómo crear reglas de cifrado, vea Definir reglas de flujo de correo [para cifrar mensajes de correo electrónico en Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

