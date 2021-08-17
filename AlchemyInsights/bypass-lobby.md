---
title: Omitir lobby
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
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059613"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlar la configuración de la sala de espera y el nivel de participación en Teams

Si desea permitir que todos, incluidos los usuarios de acceso telefónico, externos y anónimos, omita la sala de **espera,** use PowerShell para realizar esta tarea. Este es un ejemplo de modificación de la directiva de reunión global para su organización.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Actualmente, este cmdlet requiere el uso de Skype Empresarial módulo de PowerShell. Para configurarse para usar este cmdlet, consulte [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Una vez que haya configurado una directiva, debe aplicarla a los usuarios; o, si ha modificado la directiva global, se aplicará automáticamente a los usuarios. Para cualquier cambio de directiva, debe esperar al menos 4 horas hasta **24** horas para que las directivas entren en vigor. 

Asegúrese de revisar la documentación siguiente antes de realizar estos cambios para comprender exactamente lo que esto permite.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Descripción de Teams directiva de la sala de espera de reuniones

Estos valores controlan qué participantes de la reunión esperan en la sala de espera antes de ser admitidos en la reunión y el nivel de participación que se les permite en una reunión. Puede usar PowerShell para actualizar la configuración de directiva de reunión que aún no se ha implementado (etiquetada "próximamente") en el Centro de administración Teams reuniones. Vea a continuación un cmdlet de PowerShell de ejemplo que permite a todos los usuarios omitir la sala de espera.

- [Admitir automáticamente a las](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) personas es una directiva por organizador que controla si las personas se unen a una reunión directamente o esperan en la sala de espera hasta que un usuario autenticado los admita.

- [Permitir](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) que personas anónimas inicien una reunión es una directiva por organizador que controla si las personas anónimas, incluidos B2B y los usuarios federados, pueden unirse a la reunión del usuario sin un usuario autenticado de la organización que asista.

- [Permitir](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) que los usuarios de acceso telefónico local omitan la sala de espera **(** próximamente ) es una directiva  por organizador que controla si las personas que marcan por teléfono se unen a la reunión directamente o esperan en la sala de espera independientemente de la configuración Admitir automáticamente personas.

- Permitir que los organizadores invalide la configuración de la sala de espera ( próximamente **)** es una directiva  por organizador que controla si el organizador de la reunión puede invalidar la configuración de la sala de espera que un administrador establece en Admitir automáticamente a las personas y Permitir que los usuarios de acceso telefónico local omitan la sala de espera cuando programe una nueva reunión. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) 

**Nota:** Lea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para obtener una introducción completa de las Microsoft Teams de reuniones.
