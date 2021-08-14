---
title: Ocultar carpetas públicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945759"
---
# <a name="hide-public-folders"></a>Ocultar carpetas públicas

**Para ocultar todo el árbol de carpetas públicas**:

Siga los pasos de [este](https://aka.ms/ControlPF) artículo para ocultar todo el árbol de carpetas públicas de usuarios específicos o de todos.

**Para ocultar una carpeta pública específica**:

1. Agregue permisos para usuarios que necesitan acceso a la carpeta pública

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Quite el elemento de usuario **Predeterminado** de la lista **permisos**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
