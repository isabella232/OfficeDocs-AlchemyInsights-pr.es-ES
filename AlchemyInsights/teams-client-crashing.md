---
title: ¿El cliente de Teams está fallando?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691124"
---
# <a name="teams-client-crashing"></a>¿El cliente de Teams está fallando?

Si el cliente de Teams está fallando, intenta lo siguiente:

- Si está usando la aplicación de escritorio de Teams, asegúrese de que la aplicación esté completamente actualizada.

- Asegúrese de que todas las [URL e intervalos de direcciones de Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sean accesibles.

- Inicie sesión con su cuenta de administrador de inquilino y compruebe el [panel de estado del servicio](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar que no exista ninguna interrupción o degradación del servicio.

- Desinstalar y volver a instalar la aplicación Teams (vínculo)
    - Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.
    - [Descargue e instale la aplicación Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy) y, si es posible, instale Teams como administrador (haga clic con el botón derecho en el instalador de Teams y seleccione "Ejecutar como administrador" si está disponible).

Si el cliente de su equipo aún se bloquea, ¿puede reproducir el problema? En ese caso:

1. Use la Grabación de acciones de usuario para capturar los pasos.
    - Cierre todas las aplicaciones innecesarias o confidenciales.
    - Inicie sesión con la cuenta de usuario afectada, abra la Grabación de acciones de usuario y reproduzca el problema.
    - [Recopile los registros de los equipos que capturen los pasos de reproducción grabados](https://docs.microsoft.com/microsoftteams/log-files). **Nota**: Asegúrese de capturar la dirección de inicio de sesión del usuario afectado.
    - Recopile la información de la copia de seguridad y/o el depósito con errores (Windows). Inicie Windows PowerShell en la máquina en donde se produce el bloqueo y ejecute los siguientes comandos:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Anexe el archivo a su caso de soporte técnico.
