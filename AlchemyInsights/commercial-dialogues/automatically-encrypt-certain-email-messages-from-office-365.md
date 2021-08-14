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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988852"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Cifrar automáticamente determinados mensajes de correo electrónico de office 365

1. En el [Centro Exchange administración,](https://outlook.office365.com/ecp/)elija **flujo de correo > reglas**. 
2. Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar Cifrado de mensajes de Office 365 protección de derechos y derechos a los **mensajes**.
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

Para obtener más información acerca de la creación de reglas para el cifrado, vea [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

