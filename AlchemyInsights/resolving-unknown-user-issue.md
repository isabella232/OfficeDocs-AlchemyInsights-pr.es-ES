---
title: Resolución de problemas con usuarios desconocidos en el chat de Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "48785623"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a>Resolución de problemas con "usuario desconocido" en el chat de Microsoft Teams

A veces, un usuario quitado aparecerá como "usuario desconocido". Se trata de un [problema conocido](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).

Si ve persistentemente que los usuarios muestran como "usuario desconocido" en los chats de Microsoft Teams, pruebe y borre la memoria caché:

1.  Haga clic con el botón derecho en el icono de Microsoft Teams de la barra de tareas. Haga clic en  **salir** .
2.  Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.

Puede impedir que los usuarios anónimos se unan a reuniones asegurándose de que esperan en la sala de espera. Para obtener más información, consulte [cambiar la configuración de los participantes de una reunión de Microsoft Teams](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).
