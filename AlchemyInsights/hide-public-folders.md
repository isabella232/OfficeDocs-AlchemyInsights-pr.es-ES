---
title: Ocultar carpetas públicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294650"
---
# <a name="hide-public-folders"></a><span data-ttu-id="1a232-102">Ocultar carpetas públicas</span><span class="sxs-lookup"><span data-stu-id="1a232-102">Hide public folders</span></span>

<span data-ttu-id="1a232-103">**Para ocultar todo el árbol de carpetas públicas**:</span><span class="sxs-lookup"><span data-stu-id="1a232-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="1a232-104">Siga los pasos de [este](https://aka.ms/ControlPF) artículo para ocultar todo el árbol de carpetas públicas de usuarios específicos o de todos.</span><span class="sxs-lookup"><span data-stu-id="1a232-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="1a232-105">**Para ocultar una carpeta pública específica**:</span><span class="sxs-lookup"><span data-stu-id="1a232-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="1a232-106">Agregue permisos para usuarios que necesitan acceso a la carpeta pública</span><span class="sxs-lookup"><span data-stu-id="1a232-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="1a232-107">Quite el elemento de usuario **Predeterminado** de la lista **permisos**:</span><span class="sxs-lookup"><span data-stu-id="1a232-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
