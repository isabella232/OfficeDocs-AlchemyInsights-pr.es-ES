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
ms.openlocfilehash: ee54e2bcca4f4591b33ee805290192311f6cde09a9e453a813e9db328d19634d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945354"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Cómo agregar o quitar un delegado en Outlook para Windows

Para agregar un delegado en Outlook para Windows: 

1. Haga clic en **la pestaña** Archivo seguido de Account Configuración y, a **continuación,** elija **Delegate Access**.
2. Haga clic en **Agregar**. Si **Add** no aparece, es posible que no exista una conexión activa entre Outlook y Exchange. La Outlook de estado muestra el estado de conexión.
3. Escriba el nombre de la persona que desea designar como delegado o busque y elija el nombre en la lista de resultados de búsqueda.

    > [!NOTE]
    > El delegado debe ser una persona de la lista global de direcciones Exchange organización (GAL).
4. Haga clic en **Agregar** seguido de **Aceptar**.
5. En el **cuadro de diálogo Delegar** permisos, acepte la configuración de permisos predeterminada o seleccione niveles de acceso personalizados para Exchange carpetas.

    - Si un delegado necesita permiso para trabajar solo con solicitudes y respuestas de reunión, la configuración de permisos predeterminada, como **Delegado,** recibe copias de los mensajes relacionados con la reunión que se me envían son suficientes. Puede dejar la configuración **de permisos bandeja** de entrada en **Ninguno**. Las solicitudes de reunión y las respuestas irán directamente a la bandeja de entrada del delegado.

    > [!NOTE]
    > De forma predeterminada, al delegado se le concede **permiso editor (puede leer, crear** y modificar elementos) en la carpeta **Calendario.** Cuando el delegado responde a una reunión en su nombre, se agrega automáticamente a la **carpeta Calendario.**

5. Para enviar un mensaje para notificar al delegado de los permisos modificados, active la casilla Enviar automáticamente un mensaje para delegar que **resuma** estos permisos.
6. Si lo desea, active la casilla **Delegado puede ver mis elementos** privados.

    > [!IMPORTANT]
    > Esta configuración afecta a todas las Exchange carpetas. Esto incluye todas las carpetas Correo, Contactos, Calendario, Tareas, Notas y Diario. No hay ninguna forma de conceder acceso a elementos privados en solo carpetas especificadas.

7. Elija **Aceptar**.

    > [!NOTE]
    >
    > - Los mensajes enviados con permisos Enviar en nombre incluyen los nombres del delegado y los nombres junto a **From**. Cuando se envía un mensaje con permisos Enviar como, solo aparece su nombre.
    > - Una vez que agregue a alguien como delegado, puede agregar el buzón de correo Exchange a su perfil Outlook usuario. Para obtener instrucciones, consulte [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Para quitar un delegado en Outlook para Windows:

1. Haga clic en la **pestaña** Archivo.
2. Haga clic en **Account Configuración** seguido de **Delegate Access**.
3. Elija el nombre del delegado para el que desea cambiar los permisos y, a continuación, haga clic en **Quitar** seguido de **Aceptar**.
