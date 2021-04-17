---
title: Crear un grupo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816389"
---
# <a name="create-a-group"></a>Crear un grupo

En este tema se describe la creación de grupos.

**Permiso para crear un grupo**

Asegúrese de que está autorizado a crear un nuevo grupo. Los administradores globales pueden deshabilitar la creación de grupos en Azure Portal o el Panel de acceso. Puede que necesite que un administrador cree el nuevo grupo o que le conceda los permisos adecuados.

**Administrar los permisos de creación de grupos**

1. Los administradores globales pueden administrar permisos de creación de grupos (por motivos relacionados con la seguridad) u grupos de Office 365 creados en Azure Portal o el Panel de acceso, seleccionando "Los usuarios pueden crear grupos de seguridad en Azure Portals" o "Los usuarios pueden crear grupos de Office 365 en Azure Portals" en Todos los grupos  >  **Generales (Configuración).**
2. También puede restringir la creación de grupos para seleccionar un grupo de usuarios si tiene una licencia de Azure Active Directory P1 Premium.

**Deshabilitar la notificación de bienvenida para los nuevos miembros del grupo de Office 365**

La notificación de bienvenida enviada a los usuarios que se agregan a grupos de Office 365 se puede deshabilitar estableciendo **UnifiedGroupWelcomeMessageEnabled** en False en Powershell. Obtenga información sobre esta configuración [aquí](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

