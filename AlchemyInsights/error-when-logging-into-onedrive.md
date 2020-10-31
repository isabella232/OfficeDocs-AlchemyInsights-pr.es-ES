---
title: error de 0x8004de40 al iniciar OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816024"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>error de 0x8004de40 al iniciar OneDrive

Si recibe un error **0x8004de40** al iniciar sesión en OneDrive, reinicie el equipo mientras está conectado a su dominio profesional o educativo. Si recibe este error después de reiniciar, pruébelo mientras está conectado a su dominio profesional o educativo:

1. Haga clic en Inicio y escriba **cmd** o **símbolo del sistema**  en el cuadro de búsqueda, haga clic con el botón secundario en la aplicación de símbolo del sistema y seleccione  **Ejecutar como administrador** . Si se le pide una contraseña de administrador o una confirmación, escriba la contraseña o haga clic en **permitir** .  

2. En la ventana del símbolo del sistema, escriba **dsregcmd/Leave**  y espere a que se complete el comando. A continuación, escriba **dsregcmd/join** y espere a que se complete el comando.
3. Reinicie el equipo.
