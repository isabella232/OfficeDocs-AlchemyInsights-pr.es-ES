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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947534"
---
# <a name="comments-on-list-items"></a>Comentarios en elementos de lista

Los usuarios pronto podrán agregar y eliminar comentarios en los elementos de lista. Los usuarios pueden ver todos los comentarios de un elemento de lista y filtrar entre las vistas que muestran comentarios o actividades relacionadas con un elemento.

**Intervalos** :

**Versión dirigida** : implementación gradual en mediados de octubre y prevista para completar a mediados de noviembre

**Versión estándar** : implementación gradual en Mid-noviembre y espera que finalice antes de diciembre

**Implementación** : versión dirigida para toda la organización

Los usuarios deben tener en cuenta lo siguiente para poder agregar y eliminar comentarios:

- Los comentarios siguen la configuración de permisos inherente a SharePoint.
- Las listas clásicas que aún no se han creado para que se muestren en las interfaces de usuario modernas, como las listas de tareas, no tendrán esta característica de comentarios.
- La publicación de comentarios sobre listas en Microsoft Teams no está disponible en esta versión.
- Los comentarios no se indizan mediante la búsqueda.

Los administradores pueden deshabilitar esta característica en el nivel de la organización cambiando el parámetro **CommentsOnListItemsDisabled** en el cmdlet de PowerShell **set-SPOTenant** .

Actualmente no se pueden deshabilitar los comentarios en el nivel de sitio o lista. Esperamos que esos controles estén en una actualización posterior, probablemente en el primer trimestre del 2021.
