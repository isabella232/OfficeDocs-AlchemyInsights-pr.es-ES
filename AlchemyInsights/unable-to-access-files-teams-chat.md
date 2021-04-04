---
title: No se puede acceder a los archivos compartidos en el chat de Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505970"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="1876a-102">No se puede acceder a los archivos compartidos en el chat de Teams</span><span class="sxs-lookup"><span data-stu-id="1876a-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="1876a-103">En Microsoft Teams, un archivo compartido por un usuario en una ventana de chat automáticamente es almacenado en el sitio de OneDrive del usuario que comparte.</span><span class="sxs-lookup"><span data-stu-id="1876a-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="1876a-104">Cuando otro usuario intenta abrir el archivo en Teams y recibe el mensaje de error "No tiene acceso a este archivo", el problema se produce porque la característica de modo de bloqueo de permisos de usuario de acceso limitado está activada en el sitio de OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1876a-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="1876a-105">Para obtener instrucciones para deshabilitar la característica en el sitio de OneDrive, vea [Error al abrir un archivo en Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span><span class="sxs-lookup"><span data-stu-id="1876a-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="1876a-106">Compruebe si otro usuario tiene acceso al sitio de OneDrive y proporcione acceso siguiendo las instrucciones que se indican en [Compartir archivos y carpetas de OneDrive](https://go.microsoft.com/fwlink/?linkid=2156017).</span><span class="sxs-lookup"><span data-stu-id="1876a-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>