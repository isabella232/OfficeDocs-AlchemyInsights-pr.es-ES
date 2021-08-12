---
title: Configuración de la directiva de reunión
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
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925182"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrar directivas de reuniones en Microsoft Teams

**Nota: Los cambios de directiva pueden tardar hasta 24 horas en tener efecto para los usuarios.** Es posible que no pueda realizar cambios en las directivas recién creadas inmediatamente; espere 4 horas e intente modificar una directiva recién creada de nuevo.

Las directivas de reunión se usan para controlar las características disponibles para sus participantes en reuniones programadas por usuarios de la organización. Es posible que algunas características de las directivas de reunión no se implementen todavía en el centro de administración de Teams (estas se etiquetan "próximamente" en la documentación). En este caso, o si recibe un error como "No podemos actualizar la directiva en este momento, pero inténtelo de nuevo más tarde" en el Centro de administración de Microsoft Teams, se recomienda usar PowerShell para crear o modificar directivas de reunión de Teams. 

Para obtener más información acerca de las directivas de reunión, vea los siguientes recursos:

- Para obtener información sobre cómo crear directivas, realizar cambios y asignar usuarios a la directiva, vea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para realizar cambios de directiva con cmdlets de PowerShell, [vea Teams Información general de PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Debe usar el módulo Skype Empresarial [PowerShell para](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) las Teams de reuniones. 
    - Revise la [documentación de los cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obtener más información.

