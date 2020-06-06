---
title: 'Problema de activación: no se puede conectar ahora'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581892"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="09dca-102">Corrección del mensaje "no se puede conectar ahora?" de las aplicaciones de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="09dca-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="09dca-103">Si recibe este mensaje, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="09dca-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="09dca-104">Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no están bloqueando el acceso a Internet a las aplicaciones de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="09dca-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="09dca-105">Vea [direcciones URL de Microsoft e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="09dca-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="09dca-106">Vaya a **Inicio**  >  **Ejecutar**y, a continuación, escriba **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="09dca-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="09dca-107">Asegúrese de que se están ejecutando todos los servicios siguientes:</span><span class="sxs-lookup"><span data-stu-id="09dca-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="09dca-108">Configuración automática de dispositivos conectados a la red</span><span class="sxs-lookup"><span data-stu-id="09dca-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="09dca-109">Servicio de lista de redes</span><span class="sxs-lookup"><span data-stu-id="09dca-109">Network List Service</span></span>
    - <span data-ttu-id="09dca-110">Reconocimiento de ubicación de red</span><span class="sxs-lookup"><span data-stu-id="09dca-110">Network Location Awareness</span></span>
    - <span data-ttu-id="09dca-111">Registro de eventos de Windows</span><span class="sxs-lookup"><span data-stu-id="09dca-111">Windows Event Log</span></span>

<span data-ttu-id="09dca-112">Si uno de estos servicios no se está ejecutando, intente iniciarlo.</span><span class="sxs-lookup"><span data-stu-id="09dca-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="09dca-113">Si tiene un problema para iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:</span><span class="sxs-lookup"><span data-stu-id="09dca-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="09dca-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="09dca-114">**sfc /scannow**</span></span>

<span data-ttu-id="09dca-115">Una vez finalizado este comando, reinicie el equipo.</span><span class="sxs-lookup"><span data-stu-id="09dca-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="09dca-116">Para obtener información detallada, consulte ["lo sentimos, no podemos conectarnos a su cuenta. Intente de nuevo más tarde "al activar Office desde Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="09dca-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>