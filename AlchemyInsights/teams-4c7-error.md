---
title: Error de 4c7 de Teams
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700220"
---
# <a name="4c7-error-in-microsoft-teams"></a>error de 4c7 en Microsoft Teams

Este error se produce porque Microsoft Teams requiere la autenticación mediante formularios. Al implementar los servicios de Federación de Active Directory (AD FS), la autenticación de formularios no está habilitada para la intranet de forma predeterminada. Si se produce un error en la autenticación integrada de Windows, se le pedirá que inicie sesión con la autenticación de formularios.

Para resolver este problema, habilite la autenticación mediante formularios con el complemento Microsoft Management Console (MMC) de AD FS en el equipo que tiene la copia local de Active Directory. Para ello, siga estos pasos: 

1. En el panel de navegación, vaya a **directivas de autenticación**.
2. En **acciones** en el panel de detalles, seleccione **Editar autenticación principal global**.
3. En la pestaña **intranet** , seleccione **autenticación de formularios**.
4. Seleccione **Aceptar** (o **aplicar**).