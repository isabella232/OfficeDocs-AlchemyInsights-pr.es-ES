---
title: Error de Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786686"
---
# <a name="4c7-error-in-microsoft-teams"></a>Error 4c7 en Microsoft Teams

Este error se produce porque Microsoft Teams requiere autenticación de formularios. Al implementar servicios de federación de Active Directory (AD FS), la autenticación de formularios no está habilitada para la intranet de forma predeterminada. Si se produce un error en la autenticación integrada de Windows, se te pedirá que inicies sesión con la autenticación de formularios.

Para resolver este problema, habilite la autenticación de formularios mediante el complemento AD FS Microsoft Management Console (MMC) en el equipo que tiene la copia local de Active Directory. Para ello, siga estos pasos: 

1. En el panel de navegación, vaya a **Directivas de autenticación**.
2. En **Acciones** en el panel de detalles, seleccione **Editar autenticación principal global**.
3. En la **pestaña Intranet,** seleccione **Autenticación de formularios**.
4. Seleccione **Aceptar** (o **Aplicar**).