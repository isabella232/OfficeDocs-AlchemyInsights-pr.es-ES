---
title: 0x8004de40 error al iniciar OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813669"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 error al iniciar OneDrive

Si recibe un **error** 0x8004de40 al iniciar sesión en OneDrive, reinicie el equipo mientras está conectado al dominio de trabajo o escuela. Si recibe este error después de reiniciar, pruébalo mientras está conectado al dominio de trabajo o escuela:

1. Haga clic en Inicio y escriba **cmd** **o** símbolo del sistema en el cuadro de búsqueda, haga clic con el botón secundario en la aplicación del símbolo del sistema y seleccione Ejecutar como **administrador.** Si se le pide una contraseña de administrador o una confirmación, escriba la contraseña o haga clic en **Permitir**.  

2. En la ventana Símbolo del sistema, escriba **dsregcmd /leave**  y espere a que se complete el comando. A **continuación, escriba dsregcmd /join** y espere a que se complete el comando.
3. Reinicie el equipo.
