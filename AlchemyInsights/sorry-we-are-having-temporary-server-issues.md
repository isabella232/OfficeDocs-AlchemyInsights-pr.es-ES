---
title: Corrección de las aplicaciones de Microsoft 365 lo sentimos, tenemos mensajes de problemas de servidor temporales
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758262"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="fbf84-102">Corrección de las aplicaciones de 365 de Microsoft "el mensaje" tenemos problemas con el servidor temporal "</span><span class="sxs-lookup"><span data-stu-id="fbf84-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="fbf84-103">Si recibe este mensaje, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="fbf84-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fbf84-104">Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no están bloqueando el acceso a Internet a las aplicaciones de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fbf84-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="fbf84-105">Consulte [direcciones URL e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fbf84-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fbf84-106">Vaya a **Inicio**  >  **Ejecutar**y, a continuación, escriba **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="fbf84-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fbf84-107">Asegúrese de que se están ejecutando todos los servicios siguientes:</span><span class="sxs-lookup"><span data-stu-id="fbf84-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fbf84-108">Configuración automática de dispositivos conectados a la red</span><span class="sxs-lookup"><span data-stu-id="fbf84-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fbf84-109">Servicio de lista de redes</span><span class="sxs-lookup"><span data-stu-id="fbf84-109">Network List Service</span></span>
    - <span data-ttu-id="fbf84-110">Reconocimiento de ubicación de red</span><span class="sxs-lookup"><span data-stu-id="fbf84-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fbf84-111">Registro de eventos de Windows</span><span class="sxs-lookup"><span data-stu-id="fbf84-111">Windows Event Log</span></span>

<span data-ttu-id="fbf84-112">Si uno de estos servicios no se está ejecutando, intente iniciarlo.</span><span class="sxs-lookup"><span data-stu-id="fbf84-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fbf84-113">Si tiene un problema para iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:</span><span class="sxs-lookup"><span data-stu-id="fbf84-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fbf84-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="fbf84-114">**sfc /scannow**</span></span>

<span data-ttu-id="fbf84-115">Una vez finalizado este comando, reinicie el equipo.</span><span class="sxs-lookup"><span data-stu-id="fbf84-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fbf84-116">Para obtener información detallada, consulte ["lo sentimos, no podemos conectarnos a su cuenta. Intente de nuevo más tarde "al activar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fbf84-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>