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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929322"
---
# <a name="create-a-group"></a>Crear un grupo

En este tema se describe la creación de grupos.

**Permiso para crear un grupo**

Asegúrese de que está autorizado a crear un nuevo grupo. Los administradores globales pueden deshabilitar la creación de grupos en Azure Portal o el Panel de acceso. Puede que necesite que un administrador cree el nuevo grupo o que le conceda los permisos adecuados.

**Administrar los permisos de creación de grupos**

1. Los administradores globales pueden administrar permisos de creación de grupos (por motivos relacionados con la seguridad) o grupos de Office 365 creados en Azure Portal o el Panel de acceso, seleccionando "Los usuarios pueden crear grupos de seguridad en Azure Portals" o las opciones "Los usuarios pueden crear grupos Office 365 en Azure Portals" en Todos los grupos   >  **Generales (Configuración).**
2. También puede restringir la creación de grupos para seleccionar un grupo de usuarios si tiene una Azure Active Directory P1 Premium licencia.

**Deshabilitar la notificación de bienvenida para nuevos miembros Office 365 grupo**

La notificación de bienvenida enviada a los usuarios que se agregan a Office 365 pueden deshabilitarse estableciendo **UnifiedGroupWelcomeMessageEnabled** en False en Powershell. Obtenga información sobre esta configuración [aquí](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

