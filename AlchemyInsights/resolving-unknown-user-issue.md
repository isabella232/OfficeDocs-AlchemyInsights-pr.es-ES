---
title: Resolver el problema con el usuario desconocido en Teams chat
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
ms.openlocfilehash: 276a073a7213bca4a66dc6b9f27b6c9270a2845c9f2b3aaee791ce28f17e9a75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109941"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a>Resolver el problema con "Usuario desconocido" en el chat Teams chat

En ocasiones, un usuario eliminado aparecerá como "Usuario desconocido". Este es un [problema conocido](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).

Si ve usuarios que se muestran de forma persistente como "Usuario desconocido" en Teams chats, intente borrar la memoria caché:

1.  Haga clic con el botón secundario en Teams icono de la barra de tareas. Haga clic  **en Salir**.
2.  Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.

Puede impedir que los usuarios anónimos se unan a reuniones asegurándose de que esperan en la sala de espera. Para obtener más información, vea [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).
