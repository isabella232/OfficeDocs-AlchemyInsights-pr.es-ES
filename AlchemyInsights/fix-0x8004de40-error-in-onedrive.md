---
title: Corregir 0x8004de40 error en OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649765"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corregir 0x8004de40 error en OneDrive

Si estás ejecutando Windows 7 y recibes este error, actualiza para habilitar [TLS 1.1 y TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)como protocolos seguros predeterminados en WinHTTP en Windows .

Si estás ejecutando Windows 10 y recibes un 0x8004de40 error con OneDrive:

- Reinicie el equipo afectado mientras está conectado al dominio de directorio de Acitve.
- Si un reinicio no soluciona el problema, desenlace y vuelva a unirse al dispositivo desde Azure AD. 

**Nota:** Debe estar en la red corporativa mientras realiza estos pasos. No realice estos pasos cuando no esté conectado a la infraestructura corporativa (por ejemplo, mientras viaja). 

1. Abra un símbolo del sistema con privilegios elevados **seleccionando Inicio**, haga clic con el botón secundario en Símbolo del sistema y, a continuación, **seleccione Ejecutar como administrador**. 

1. Escriba *dsregcmd /leave y* presione **Entrar**.

1. Cuando haya finalizado, escriba *dsregcmd /join y* presione **Entrar**.

1. Cuando se complete, cierre el símbolo del sistema.

1. Reinicie el equipo e inicie sesión en OneDrive.