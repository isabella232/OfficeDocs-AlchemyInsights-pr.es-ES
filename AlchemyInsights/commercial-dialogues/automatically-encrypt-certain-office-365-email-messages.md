---
title: Cifrar automáticamente ciertos mensajes Office 365 de correo electrónico
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
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949584"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Cifrar automáticamente ciertos mensajes Office 365 de correo electrónico

Puede cifrar automáticamente los mensajes que los usuarios envían a determinadas personas u organizaciones externas. Para ello, realice los siguientes pasos:

1. En el [Centro Exchange administración,](https://outlook.office365.com/ecp/)elija **flujo de correo > reglas**. 
2. Haga clic **en el icono Nuevo (+)** y, a continuación, haga clic en Aplicar Cifrado de mensajes de Office 365 protección de derechos y derechos a los **mensajes**.
3. En **Nombre**, escriba un nombre para la regla, como *Cifrar mensajes enviados a DrToniRamos@gmail.com*.
4. En **Aplicar esta regla si**, elija El destinatario > es esta **persona**. 
5. En la **ventana Seleccionar miembros,** seleccione el nombre de la persona a la que desea que se aplique la regla de cifrado y, a continuación, haga clic en **Agregar**. 
6. Cuando haya terminado de agregar usuarios, haga clic en **Aceptar**.
7. Junto al campo **Hacer lo siguiente,** haga clic **en Seleccionar uno**. 
8. En el **menú desplegable Plantilla RMS,** seleccione **Cifrar** y, a continuación, haga clic en **Aceptar**. (Si no ve esta opción, significa que el plan no incluye cifrado automático. Pero puedes agregarlo!
9. Elija cualquier selección opcional (de una lista de selecciones opcionales que puede realizar en este momento, muchas de las cuales se pueden dejar con la configuración predeterminada para simplificar).
10. Haga clic en **Guardar**.

> [!IMPORTANT]
> Siempre puede volver y editar esta regla más adelante.

Para obtener más información acerca de cómo crear reglas de cifrado, vea Definir reglas de flujo de correo para cifrar mensajes de correo [electrónico en Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

