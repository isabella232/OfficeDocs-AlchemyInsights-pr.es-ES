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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946596"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 error al iniciar OneDrive

Si recibe un **error** 0x8004de40 al iniciar sesión en OneDrive, reinicie el equipo mientras está conectado al dominio de trabajo o escuela. Si recibe este error después de reiniciar, pruébalo mientras está conectado al dominio de trabajo o escuela:

1. Haga clic en Inicio y escriba **cmd** **o** símbolo del sistema en el cuadro de búsqueda, haga clic con el botón secundario en la aplicación del símbolo del sistema y seleccione Ejecutar como **administrador.** Si se le pide una contraseña de administrador o una confirmación, escriba la contraseña o haga clic en **Permitir**.  

2. En la ventana Símbolo del sistema, escriba **dsregcmd /leave**  y espere a que se complete el comando. A **continuación, escriba dsregcmd /join** y espere a que se complete el comando.
3. Reinicie el equipo.
