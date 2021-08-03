---
title: Habilitar los seminarios web de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: a56abdaae182b840a1a96466e0581ef49b2b0075
ms.sourcegitcommit: 540a4e2515f7cfddee65519046454fc4437cd287
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/01/2021
ms.locfileid: "53688991"
---
# <a name="enable-teams-webinars"></a>Habilitar los seminarios web de Teams

El registro del seminario web está habilitado de forma predeterminada. Si desea desactivar el registro de reuniones, puede usar el Centro de administración de Teams: 

1. Vaya al [Centro de administración de Teams](https://admin.teams.microsoft.com/policies/meetings). 

2. Seleccione la directiva **Global (predeterminada para toda la organización)** u otra directiva específica. 

3. En **General**, establezca **Permitir registro de reuniones** en **Desactivado**. 

Cuando el registro de la reunión se establece en **Activado**, también puede administrar quién se registra en los seminarios web de Teams mediante el Centro de administración de Teams: 

1. Vaya al [Centro de administración de Teams](https://admin.teams.microsoft.com/policies/meetings). 

2. Seleccione la directiva **Global (predeterminada para toda la organización)** u otra directiva específica. 

3. En **General**, vaya a la configuración **Quién puede registrarse** y seleccione **Todos** o **Todos los usuarios de la empresa**. 

**Nota**: si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web. Para obtener más información sobre cómo habilitar esta configuración, consulte [Administrar la configuración de reuniones en Microsoft Teams](/microsoftteams/meeting-settings-in-teams). 

Para obtener más información sobre cómo configurar quién puede registrarse en seminarios web y cómo administrar estas directivas con PowerShell de Teams, consulte [Configurar quién puede registrarse en seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obtener más información sobre la configuración de Listas Microsoft, consulte [Configuración del control para Listas Microsoft](/sharepoint/control-lists). 