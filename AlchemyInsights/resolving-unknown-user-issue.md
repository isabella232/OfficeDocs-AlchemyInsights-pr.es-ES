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
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="e6bb5-102">Resolución de problemas con "usuario desconocido" en el chat de Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e6bb5-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="e6bb5-103">A veces, un usuario quitado aparecerá como "usuario desconocido".</span><span class="sxs-lookup"><span data-stu-id="e6bb5-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="e6bb5-104">Se trata de un [problema conocido](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span><span class="sxs-lookup"><span data-stu-id="e6bb5-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="e6bb5-105">Si ve persistentemente que los usuarios muestran como "usuario desconocido" en los chats de Microsoft Teams, pruebe y borre la memoria caché:</span><span class="sxs-lookup"><span data-stu-id="e6bb5-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="e6bb5-106">Haga clic con el botón derecho en el icono de Microsoft Teams de la barra de tareas.</span><span class="sxs-lookup"><span data-stu-id="e6bb5-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="e6bb5-107">Haga clic en  **salir** .</span><span class="sxs-lookup"><span data-stu-id="e6bb5-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="e6bb5-108">Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.</span><span class="sxs-lookup"><span data-stu-id="e6bb5-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="e6bb5-109">Puede impedir que los usuarios anónimos se unan a reuniones asegurándose de que esperan en la sala de espera.</span><span class="sxs-lookup"><span data-stu-id="e6bb5-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="e6bb5-110">Para obtener más información, consulte [cambiar la configuración de los participantes de una reunión de Microsoft Teams](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span><span class="sxs-lookup"><span data-stu-id="e6bb5-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
