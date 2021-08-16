---
title: Cifrar automáticamente los Office 365 de correo electrónico enviados a determinados dominios
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082203"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Cifrar automáticamente los Office 365 de correo electrónico enviados a determinados dominios

1. En el [Centro Exchange administración,](https://outlook.office365.com/ecp/)elija **flujo de correo > reglas**. 
2. Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar Cifrado de mensajes de Office 365 protección de derechos y derechos a los **mensajes**.
3. En **Nombre**, escriba un nombre para la regla, como *Cifrar mensajes enviados* a contoso.com .
4. En **Aplicar esta regla si**, elija El destinatario > dominio **es**. 
5. Escriba el nombre del dominio, como **contoso.com**.
6. Haga clic **en el icono Agregar (+)** y, a continuación, haga clic en **Aceptar**.
7. Junto al campo **Hacer lo siguiente,** haga clic **en Seleccionar uno**. 
8. En el **menú desplegable Plantilla RMS,** seleccione **Cifrar** y, a continuación, haga clic en **Aceptar**. (Si no ve esta opción, significa que el plan no incluye cifrado automático. Pero puedes agregarlo!
9. Elija cualquier selección opcional (de una lista de selecciones opcionales que puede realizar en este momento, muchas de las cuales se pueden dejar con la configuración predeterminada para simplificar).
10. Haga clic en **Guardar**.

> [!IMPORTANT]
> Siempre puede volver y editar esta regla más adelante.

Para obtener más información acerca de la creación de reglas para el cifrado, vea [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)