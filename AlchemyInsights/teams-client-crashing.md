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
# <a name="teams-client-crashing"></a><span data-ttu-id="7584f-102">¿El cliente de Teams está fallando?</span><span class="sxs-lookup"><span data-stu-id="7584f-102">Teams client crashing?</span></span>

<span data-ttu-id="7584f-103">Si el cliente de Teams está fallando, intenta lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="7584f-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="7584f-104">Si está usando la aplicación de escritorio de Teams, asegúrese de que la aplicación esté completamente actualizada.</span><span class="sxs-lookup"><span data-stu-id="7584f-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="7584f-105">Asegúrese de que todas las [URL e intervalos de direcciones de Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sean accesibles.</span><span class="sxs-lookup"><span data-stu-id="7584f-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="7584f-106">Inicie sesión con su cuenta de administrador de inquilino y compruebe el [panel de estado del servicio](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar que no exista ninguna interrupción o degradación del servicio.</span><span class="sxs-lookup"><span data-stu-id="7584f-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="7584f-107">Desinstalar y volver a instalar la aplicación Teams (vínculo)</span><span class="sxs-lookup"><span data-stu-id="7584f-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="7584f-108">Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.</span><span class="sxs-lookup"><span data-stu-id="7584f-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="7584f-109">[Descargue e instale la aplicación Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy) y, si es posible, instale Teams como administrador (haga clic con el botón derecho en el instalador de Teams y seleccione "Ejecutar como administrador" si está disponible).</span><span class="sxs-lookup"><span data-stu-id="7584f-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="7584f-110">Si el cliente de su equipo aún se bloquea, ¿puede reproducir el problema?</span><span class="sxs-lookup"><span data-stu-id="7584f-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="7584f-111">En ese caso:</span><span class="sxs-lookup"><span data-stu-id="7584f-111">If so:</span></span>

1. <span data-ttu-id="7584f-112">Use la Grabación de acciones de usuario para capturar los pasos.</span><span class="sxs-lookup"><span data-stu-id="7584f-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="7584f-113">Cierre todas las aplicaciones innecesarias o confidenciales.</span><span class="sxs-lookup"><span data-stu-id="7584f-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="7584f-114">Inicie sesión con la cuenta de usuario afectada, abra la Grabación de acciones de usuario y reproduzca el problema.</span><span class="sxs-lookup"><span data-stu-id="7584f-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="7584f-115">[Recopile los registros de los equipos que capturen los pasos de reproducción grabados](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="7584f-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="7584f-116">**Nota**: Asegúrese de capturar la dirección de inicio de sesión del usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="7584f-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="7584f-117">Recopile la información de la copia de seguridad y/o el depósito con errores (Windows).</span><span class="sxs-lookup"><span data-stu-id="7584f-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="7584f-118">Inicie Windows PowerShell en la máquina en donde se produce el bloqueo y ejecute los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7584f-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="7584f-119">Anexe el archivo a su caso de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="7584f-119">Attach the file to your support case.</span></span>
