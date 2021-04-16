---
title: 'Problema de activación: no podemos conectarnos en este momento'
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806459"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="e68d8-102">Corregir el mensaje de aplicaciones de Microsoft 365 "No podemos conectarnos en este momento"</span><span class="sxs-lookup"><span data-stu-id="e68d8-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="e68d8-103">Si recibe este mensaje, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="e68d8-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e68d8-104">Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a las aplicaciones de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e68d8-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e68d8-105">Consulte [Direcciones URL de Microsoft e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e68d8-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e68d8-106">Vaya a **Iniciar**  >  **ejecución** y, a continuación, escriba **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="e68d8-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e68d8-107">Asegúrese de que todos los servicios siguientes están en ejecución:</span><span class="sxs-lookup"><span data-stu-id="e68d8-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e68d8-108">Configuración automática de dispositivos conectados en red</span><span class="sxs-lookup"><span data-stu-id="e68d8-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e68d8-109">Servicio de lista de red</span><span class="sxs-lookup"><span data-stu-id="e68d8-109">Network List Service</span></span>
    - <span data-ttu-id="e68d8-110">Reconocimiento de ubicación de red</span><span class="sxs-lookup"><span data-stu-id="e68d8-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e68d8-111">Registro de eventos de Windows</span><span class="sxs-lookup"><span data-stu-id="e68d8-111">Windows Event Log</span></span>

<span data-ttu-id="e68d8-112">Si uno de estos servicios no se está ejecutando, intente iniciarlo.</span><span class="sxs-lookup"><span data-stu-id="e68d8-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e68d8-113">Si tiene un problema al iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:</span><span class="sxs-lookup"><span data-stu-id="e68d8-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e68d8-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="e68d8-114">**sfc /scannow**</span></span>

<span data-ttu-id="e68d8-115">Cuando finalice este comando, reinicie el equipo.</span><span class="sxs-lookup"><span data-stu-id="e68d8-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e68d8-116">Para obtener información detallada, consulta ["Lo sentimos, no podemos conectarnos a tu cuenta. Vuelva a intentarlo más adelante" error al activar Office desde Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e68d8-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>