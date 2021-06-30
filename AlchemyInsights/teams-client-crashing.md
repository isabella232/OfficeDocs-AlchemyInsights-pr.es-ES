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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187738"
---
# <a name="teams-client-crashing"></a>El cliente de Teams se bloquea

Si el cliente de Teams está fallando, intenta lo siguiente:

- Si está usando la aplicación de escritorio de Teams, asegúrese de que la aplicación esté completamente actualizada.

- Asegúrese de que todas las [URL e intervalos de direcciones de Microsoft 365](/microsoftteams/connectivity-issues) sean accesibles.

- Inicie sesión con su cuenta de administrador de inquilino y compruebe el [panel de estado del servicio](/office365/enterprise/view-service-health) para verificar que no exista ninguna interrupción o degradación del servicio.

- Desinstalar y reinstalar la aplicación de Teams
    - Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.
    - [Descargue e instale la aplicación Teams](https://www.microsoft.com/microsoft-teams/download-app) y si es posible instale Teams como administrador (haga clic con el botón derecho en el instalador de Teams y seleccione **"Ejecutar como administrador" si está disponible)**.

Si el cliente de Teams sigue bloqueándose, intente reproducir el problema. Si puede:

1. Use la Grabación de acciones de usuario para capturar los pasos.
    - Cierre todas las aplicaciones innecesarias o confidenciales.
    - Inicie sesión con la cuenta de usuario afectada, abra la Grabación de acciones de usuario y reproduzca el problema.
    - [Recopile los registros de los equipos que capturen los pasos de reproducción grabados](/microsoftteams/log-files). **Nota**: Asegúrese de capturar la dirección de inicio de sesión del usuario afectado.
    - Recopile la información de la copia de seguridad y/o el depósito con errores (Windows). Inicie Windows PowerShell en el equipo donde se produce el bloqueo y ejecute los siguientes comandos (después de cada comando, presione Entrar):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Después de generar el archivo de texto y aparecer en la pantalla, guárdelo y adjunte a la solicitud de servicio. 
