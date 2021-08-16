---
title: Teams error de 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049325"
---
# <a name="4c7-error-in-microsoft-teams"></a>Error 4c7 en Microsoft Teams

Este error se produce porque Microsoft Teams requiere autenticación de formularios. Al implementar servicios de federación de Active Directory (AD FS), la autenticación de formularios no está habilitada para la intranet de forma predeterminada. Si Windows la autenticación integrada falla, se le pedirá que inicie sesión con la autenticación de formularios.

Para resolver este problema, habilite la autenticación de formularios mediante el complemento AD FS Microsoft Management Console (MMC) en el equipo que tiene la copia local de Active Directory. Para ello, siga estos pasos: 

1. En el panel de navegación, vaya a **Directivas de autenticación**.
2. En **Acciones** en el panel de detalles, seleccione **Editar autenticación principal global**.
3. En la **pestaña Intranet,** seleccione **Autenticación de formularios**.
4. Seleccione **Aceptar** (o **Aplicar**).