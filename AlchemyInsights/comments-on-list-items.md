---
title: Comentarios en elementos de lista
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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724171"
---
# <a name="comments-on-list-items"></a>Comentarios en elementos de lista

Los usuarios pueden ver todos los comentarios de un elemento de lista y filtrar entre las vistas que muestran comentarios o actividades relacionadas con un elemento.

Los usuarios deben tener en cuenta lo siguiente para poder agregar y eliminar comentarios:

- Los comentarios siguen la configuración de permisos inherente a SharePoint.
- Las listas clásicas que aún no se han creado para que se muestren en las interfaces de usuario modernas, como las listas de tareas, no tendrán esta característica de comentarios.
- La publicación de comentarios sobre listas en Microsoft Teams no está disponible en esta versión.
- Los comentarios no se indizan mediante la búsqueda.

Los administradores pueden deshabilitar esta característica en el nivel de la organización cambiando el parámetro **CommentsOnListItemsDisabled** en el cmdlet de PowerShell **set-SPOTenant** .

Actualmente no se pueden deshabilitar los comentarios en el nivel de sitio o lista. Esperamos que esos controles estén en una actualización posterior, probablemente en el primer trimestre del 2021.
