---
title: Crear un grupo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086394"
---
# <a name="create-a-group"></a>Crear un grupo

En este tema se describe la creación de grupos.

**Permiso para crear un grupo**

Asegúrese de que tiene autorización para crear un nuevo grupo. Los administradores globales pueden deshabilitar la creación de grupos en el panel de acceso o el portal de Azure. Es posible que necesite un administrador para crear el nuevo grupo o para concederle los permisos adecuados.

**Administrar permisos de creación de grupos**

1. Los administradores globales pueden administrar los permisos de creación de grupos (por motivos relacionados con la seguridad) o los grupos de Office 365 creados en el portal de Azure o en el panel de acceso, seleccionando "los usuarios pueden crear grupos de seguridad en los portales de Azure" o "los usuarios pueden crear grupos de Office 365 en Azure portales" en **todos los grupos**  >  **General (configuración)**.
2. También puede restringir la creación de grupos para seleccionar un grupo de usuarios si tiene una licencia de Azure Premium de Active Directory P1.

**Deshabilitar la notificación de bienvenida para nuevos miembros del grupo de Office 365**

La notificación de bienvenida que se envía a los usuarios que se agregan a los grupos de Office 365 se puede deshabilitar si se establece **UnifiedGroupWelcomeMessageEnabled** en false en PowerShell. Obtenga información [aquí](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)sobre esta configuración.

