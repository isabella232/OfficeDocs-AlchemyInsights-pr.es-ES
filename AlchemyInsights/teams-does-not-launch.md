---
title: Teams no se inicia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329343"
---
# <a name="teams-doesnt-launch"></a>Teams no se inicia

Si intenta abrir Microsoft Teams pero no se inicia, pruebe lo siguiente:

1. Vaya a **%appdata%\Microsoft\Teams**.
1. Elimine el contenido de la carpeta.
1. Reinicie el equipo e intente iniciar Teams.

Es posible que tenga que reinstalar Teams. Para reinstalar:

1. Desinstale mediante el Panel de control
1. Vaya a **%appdata%\Microsoft\Teams\Application Cache**.
1. Elimine el contenido de la carpeta.
1. Vaya a **%appdata%\Microsoft\teams\Cache**.
1. Elimine el contenido de la carpeta.
1. Reinicie el equipo y, a continuación, descargue e instale Teams.

Si desea ejecutar un diagnóstico en su espacio empresarial para un usuario específico que no puede iniciar sesión, inicie una nueva búsqueda con la palabra clave **TeamsUserUnableToSignIn** y siga las indicaciones.