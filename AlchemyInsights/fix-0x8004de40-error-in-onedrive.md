---
title: Error de corrección 0x8004de40 en OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745147"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Error de corrección 0x8004de40 en OneDrive

Si recibe un error 0x8004de40 con OneDrive:

- Reinicie el equipo afectado mientras está conectado a su dominio de directorio de Acitve.
- Si un reinicio no soluciona el problema, separe y vuelva a unirse al dispositivo desde Azure AD. 

**Nota**: debe estar en la red corporativa mientras realiza estos pasos. No realice estos pasos cuando no pueda conectarse a su infraestructura corporativa (por ejemplo, mientras viaja). 

- Abra un símbolo del sistema con privilegios elevados. 
- Para abrir un símbolo del sistema con privilegios elevados, haga clic en- **iniciar**, haga clic con el botón secundario en **símbolo del sistema**y haga clic en **Ejecutar como administrador**.
- Escriba *dsregcmd/Leave* y presione **entrar**.
- Cuando termine, escriba *dsregcmd/join* y presione **entrar**.
- Cuando termine, cierre el símbolo del sistema.
- Reinicie el equipo e inicie sesión en OneDrive.