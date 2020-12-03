---
title: Recuperar un elemento que ya no está en la carpeta elementos eliminados
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "7320"
ms.openlocfilehash: b6ac084ead88b090d6caab1405d5d96f24890ea7
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560714"
---
# <a name="recover-an-item-thats-no-longer-in-your-deleted-items-folder"></a>Recuperar un elemento que ya no está en la carpeta elementos eliminados

Si no encuentra un elemento en la carpeta elementos eliminados, el siguiente punto que debe buscar es la carpeta elementos recuperables. Se trata de una carpeta oculta a la que se mueven los elementos cuando:
- Se eliminan de la carpeta elementos eliminados.
- La carpeta elementos eliminados se vacía, ya sea por usted o por una directiva establecida por el administrador de ti.
- Elimine un elemento seleccionándolo y presionando **Mayús + Supr**.

Para ver y recuperar los elementos que se han movido a la carpeta elementos recuperables:
1. En un explorador web, inicie sesión en Outlook Web App mediante la dirección URL proporcionada por la persona que administra el correo electrónico en su organización. Escriba su nombre de usuario y contraseña y, a continuación, seleccione **iniciar sesión**.
1. En la lista de carpetas de correo electrónico, haga clic con el botón secundario en **elementos eliminados** y seleccione **recuperar elementos eliminados...**
1. Si es necesario, use el cuadro de búsqueda para buscar el elemento que desee recuperar.
1. Cuando encuentre el elemento, selecciónelo y haga clic en **recuperar**.
   Los elementos recuperados se mueven a la ubicación predeterminada para cada tipo de elemento.
    - Los mensajes van a la bandeja de entrada.
    - Los elementos de calendario van a su calendario.
    - Los contactos van a la carpeta contactos.
    - Las tareas van a la carpeta tareas.

**Sugerencias para recuperar elementos de la carpeta elementos recuperables**

- La fecha de eliminación de un elemento en la carpeta elementos recuperables es cuando el elemento se movió a la carpeta elementos eliminados. No es la fecha en la que el elemento se movió a la carpeta elementos recuperables.
- Los elementos de la carpeta elementos recuperables no tienen iconos, por lo que todos son muy similares.
    - Si está buscando un contacto, busque un elemento que tenga el nombre de la persona, pero sin línea de asunto.
    - Si está buscando una cita de calendario, busque un elemento que no tenga el nombre de una persona o una línea de asunto.
    - Si está buscando un contacto, una cita de calendario o una tarea, busque el texto de ese elemento.
- Para recuperar varios elementos, mantenga el mouse sobre cada elemento y active la casilla situada junto a él, haga clic en **recuperar**. También puede recuperar varios elementos adyacentes activando la casilla de verificación del primer elemento, manteniendo presionada la tecla **MAYÚS** y, a continuación, seleccionando la casilla para el último elemento. Una vez seleccionados todos los elementos, seleccione **recuperar**.
- Puede depurar elementos de la lista **recuperar elementos eliminados** . Simplemente seleccione el elemento y, a continuación, seleccione **purgar**. Si purga un elemento, no podrá usar recuperar elementos eliminados para volver a usarlo. La purga de un mensaje no lo quita de las copias de seguridad que se realizaron antes de purgarlo.
- Es posible que su organización haya especificado cuánto tiempo los elementos de la carpeta elementos recuperables estarán disponibles para la recuperación. Por ejemplo, puede haber una directiva que elimine todo lo que haya en la carpeta elementos eliminados durante 30 días y otra directiva que le permita recuperar los elementos de la carpeta elementos recuperables durante un máximo de 14 días.
