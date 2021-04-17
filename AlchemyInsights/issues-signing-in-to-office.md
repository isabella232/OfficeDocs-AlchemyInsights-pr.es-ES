---
title: Problemas al iniciar sesión en aplicaciones de Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833056"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="83ef1-102">Pantalla de inicio de sesión en blanco en aplicaciones de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="83ef1-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="83ef1-103">Para solucionar este problema, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="83ef1-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="83ef1-104">Instalar las actualizaciones más recientes [para Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="83ef1-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="83ef1-105">Restablecer opciones de Internet Explorer: vaya a **Herramientas** Opciones de Internet Configuración avanzada de Internet Explorer (tenga en cuenta que perderá la configuración personalizada) y vuelva a intentar  >    >    >   iniciar sesión en Office.</span><span class="sxs-lookup"><span data-stu-id="83ef1-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="83ef1-106">Deshabilite Windows Defender Protección de aplicaciones (WDAG) o cualquier firewall o programa antivirus similar:</span><span class="sxs-lookup"><span data-stu-id="83ef1-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="83ef1-107">En el Panel de control, vaya **a Programas** y, a continuación, elija Activar o desactivar las características **de Windows.**</span><span class="sxs-lookup"><span data-stu-id="83ef1-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="83ef1-108">Si Windows Defender Application Guard está habilitado, intenta deshabilitarlo.</span><span class="sxs-lookup"><span data-stu-id="83ef1-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="83ef1-109">**Nota:** Es posible que deba reiniciar el equipo.</span><span class="sxs-lookup"><span data-stu-id="83ef1-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="83ef1-110">Asegúrese de que el complemento Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) no esté bloqueado por ninguna aplicación o programa antivirus o firewall.</span><span class="sxs-lookup"><span data-stu-id="83ef1-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="83ef1-111">[Borra las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el Administrador de credenciales de Windows.</span><span class="sxs-lookup"><span data-stu-id="83ef1-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="83ef1-112">**Nota:** Las rutas de acceso del Registro para Office 2016 han cambiado a 16.0.</span><span class="sxs-lookup"><span data-stu-id="83ef1-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="83ef1-113">(Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="83ef1-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="83ef1-114">Para obtener más información, vea [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="83ef1-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>