---
title: El cliente de Teams se bloquea
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890355"
---
# <a name="teams-client-crashing"></a>El cliente de Teams se bloquea

Si el cliente de Teams está fallando, intenta lo siguiente:

- Si está usando la aplicación de escritorio de Teams, asegúrese de que la aplicación esté completamente actualizada.

- Asegúrese de que todas las [URL e intervalos de direcciones de Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sean accesibles.

- Inicie sesión con su cuenta de administrador de inquilino y compruebe el [panel de estado del servicio](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar que no exista ninguna interrupción o degradación del servicio.

- Desinstalar y reinstalar la aplicación de Teams
    - Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.
    - [Descargue e instale la aplicación Teams](https://www.microsoft.com/microsoft-teams/download-app) y si es posible instale Teams como administrador (haga clic con el botón derecho en el instalador de Teams y seleccione **"Ejecutar como administrador" si está disponible)**.

Si el cliente de Teams sigue bloqueándose, intente reproducir el problema. Si le es posible, haga lo siguiente:

1. Use la Grabación de acciones de usuario para capturar los pasos.
    - Cierre todas las aplicaciones innecesarias o confidenciales.
    - Inicie sesión con la cuenta de usuario afectada, abra la Grabación de acciones de usuario y reproduzca el problema.
    - [Recopile los registros de los equipos que capturen los pasos de reproducción grabados](https://docs.microsoft.com/microsoftteams/log-files). **Nota**: Asegúrese de capturar la dirección de inicio de sesión del usuario afectado.
    - Recopile la información de la copia de seguridad o el depósito con errores (Windows). Inicie Windows PowerShell en el equipo donde se produce el bloqueo y ejecute los siguientes comandos (después de cada comando, presione Entrar):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Después de generar el archivo de texto y aparecer en la pantalla, guárdelo y adjunte a la solicitud de servicio. 
