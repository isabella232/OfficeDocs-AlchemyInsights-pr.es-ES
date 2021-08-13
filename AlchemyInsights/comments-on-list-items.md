---
title: Comentarios sobre elementos de lista
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
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995524"
---
# <a name="comments-on-list-items"></a>Comentarios sobre elementos de lista

Los usuarios pueden ver todos los comentarios de un elemento de lista y filtrar entre vistas que muestran comentarios o actividades relacionadas con un elemento.

Los usuarios deben tener en cuenta lo siguiente antes de poder agregar y eliminar comentarios:

- Los comentarios siguen la configuración de permisos inherente a SharePoint.
- Las listas clásicas que aún no están creadas para mostrarse en interfaces de usuario modernas, como las listas de tareas, no tendrán esta característica de comentarios.
- Los comentarios sobre listas de Teams no están disponibles con esta versión.
- La búsqueda no indiza los comentarios.

Los administradores pueden deshabilitar esta característica en el nivel de la organización cambiando el parámetro **CommentsOnListItemsDisabled** en el cmdlet **Set-SPOTenant** de PowerShell.

Actualmente no es posible deshabilitar los comentarios en el nivel de sitio o de lista. Esperamos tener esos controles en una actualización posterior, probablemente en el primer trimestre de 2021.
