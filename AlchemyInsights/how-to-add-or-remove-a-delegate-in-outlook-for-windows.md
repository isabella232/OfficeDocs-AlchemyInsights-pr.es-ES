---
title: Cómo agregar o quitar un delegado en Outlook para Windows
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
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571910"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Cómo agregar o quitar un delegado en Outlook para Windows

Para agregar un delegado en Outlook para Windows: 

1. Haga clic en la pestaña **archivo** seguida de **configuración** de la cuenta y, a continuación, elija **delegar acceso**.
2. Haga clic en **Agregar**. Si no aparece **Agregar** , es posible que no exista una conexión activa entre Outlook y Exchange. La barra de estado de Outlook muestra el estado de la conexión.
3. Escriba el nombre de la persona que desea designar como su delegado, o bien busque y elija el nombre en la lista de resultados de la búsqueda.

    > [!NOTE]
    > El delegado debe ser una persona de la lista global de direcciones (GAL) de Exchange de la organización.
4. Haga clic en **Agregar** seguido de **Aceptar**.
5. En el cuadro de diálogo **permisos de delegado** , acepte la configuración de permisos predeterminada o seleccione niveles de acceso personalizados para las carpetas de Exchange.

    - Si un delegado necesita permiso para trabajar solo con convocatorias de reunión y respuestas, la configuración de permisos predeterminada, como **Delegate recibe copias de los mensajes de reunión que se me envíen** es suficiente. Puede dejar la configuración de permisos de la **bandeja de entrada** en **ninguno**. Las convocatorias de reunión y las respuestas Irán directamente a la bandeja de entrada del delegado.

    > [!NOTE]
    > De forma predeterminada, el delegado tiene concedido el permiso **Editor (puede leer, crear y modificar elementos)** a la carpeta **calendario** . Cuando el delegado responde a una reunión en su nombre, se agrega automáticamente a la carpeta del **calendario** .

5. Para enviar un mensaje para notificar al delegado los permisos modificados, active la casilla de verificación **enviar automáticamente un mensaje al delegado que resume estos permisos** .
6. Si lo desea, active la casilla el **delegado puede ver mis elementos privados** .

    > [!IMPORTANT]
    > Esta configuración afecta a todas las carpetas de Exchange. Esto incluye todas las carpetas correo, contactos, calendario, tareas, notas y diario. No hay ninguna forma de conceder acceso a los elementos privados en las carpetas especificadas.

7. Elija **Aceptar**.

    > [!NOTE]
    >
    > - Los mensajes enviados con los permisos enviar en nombre de incluyen el delegado y los nombres junto a **desde**. Cuando se envía un mensaje con los permisos enviar como, sólo aparece su nombre.
    > - Una vez que agregue a alguien como delegado, puede Agregar el buzón de Exchange a su perfil de Outlook. Para obtener instrucciones, consulte [administrar los elementos de correo y calendario de otra persona](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Para quitar un delegado en Outlook para Windows:

1. Haga clic en la pestaña **archivo** .
2. Haga clic en configuración de la **cuenta** seguida de **Acceso delegado**.
3. Elija el nombre del delegado para el que desea cambiar los permisos y, a continuación, haga clic en **quitar** seguida de **Aceptar**.
