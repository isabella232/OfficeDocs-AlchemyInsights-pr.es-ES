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
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100239"
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