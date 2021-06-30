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
# <a name="teams-client-crashing"></a><span data-ttu-id="f078e-102">El cliente de Teams se bloquea</span><span class="sxs-lookup"><span data-stu-id="f078e-102">Teams client crashing</span></span>

<span data-ttu-id="f078e-103">Si el cliente de Teams está fallando, intenta lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f078e-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="f078e-104">Si está usando la aplicación de escritorio de Teams, asegúrese de que la aplicación esté completamente actualizada.</span><span class="sxs-lookup"><span data-stu-id="f078e-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="f078e-105">Asegúrese de que todas las [URL e intervalos de direcciones de Microsoft 365](/microsoftteams/connectivity-issues) sean accesibles.</span><span class="sxs-lookup"><span data-stu-id="f078e-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="f078e-106">Inicie sesión con su cuenta de administrador de inquilino y compruebe el [panel de estado del servicio](/office365/enterprise/view-service-health) para verificar que no exista ninguna interrupción o degradación del servicio.</span><span class="sxs-lookup"><span data-stu-id="f078e-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="f078e-107">Desinstalar y reinstalar la aplicación de Teams</span><span class="sxs-lookup"><span data-stu-id="f078e-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="f078e-108">Examine la carpeta %appdata%\Microsoft\teams\ en su equipo y elimine todos los archivos en ese directorio.</span><span class="sxs-lookup"><span data-stu-id="f078e-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="f078e-109">[Descargue e instale la aplicación Teams](https://www.microsoft.com/microsoft-teams/download-app) y si es posible instale Teams como administrador (haga clic con el botón derecho en el instalador de Teams y seleccione **"Ejecutar como administrador" si está disponible)**.</span><span class="sxs-lookup"><span data-stu-id="f078e-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="f078e-110">Si el cliente de Teams sigue bloqueándose, intente reproducir el problema.</span><span class="sxs-lookup"><span data-stu-id="f078e-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="f078e-111">Si puede:</span><span class="sxs-lookup"><span data-stu-id="f078e-111">If you can:</span></span>

1. <span data-ttu-id="f078e-112">Use la Grabación de acciones de usuario para capturar los pasos.</span><span class="sxs-lookup"><span data-stu-id="f078e-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="f078e-113">Cierre todas las aplicaciones innecesarias o confidenciales.</span><span class="sxs-lookup"><span data-stu-id="f078e-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="f078e-114">Inicie sesión con la cuenta de usuario afectada, abra la Grabación de acciones de usuario y reproduzca el problema.</span><span class="sxs-lookup"><span data-stu-id="f078e-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="f078e-115">[Recopile los registros de los equipos que capturen los pasos de reproducción grabados](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="f078e-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="f078e-116">**Nota**: Asegúrese de capturar la dirección de inicio de sesión del usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="f078e-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="f078e-117">Recopile la información de la copia de seguridad y/o el depósito con errores (Windows).</span><span class="sxs-lookup"><span data-stu-id="f078e-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="f078e-118">Inicie Windows PowerShell en el equipo donde se produce el bloqueo y ejecute los siguientes comandos (después de cada comando, presione Entrar):</span><span class="sxs-lookup"><span data-stu-id="f078e-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="f078e-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="f078e-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="f078e-120">Después de generar el archivo de texto y aparecer en la pantalla, guárdelo y adjunte a la solicitud de servicio.</span><span class="sxs-lookup"><span data-stu-id="f078e-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
