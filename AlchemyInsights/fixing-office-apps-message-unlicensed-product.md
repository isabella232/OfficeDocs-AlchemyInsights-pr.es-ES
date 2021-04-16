---
title: No se ha podido activar Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812589"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="99e0a-102">No se ha podido activar Office</span><span class="sxs-lookup"><span data-stu-id="99e0a-102">Unable to activate Office</span></span>

- <span data-ttu-id="99e0a-103">Compruebe el estado de la suscripción para ver si ha caducado.</span><span class="sxs-lookup"><span data-stu-id="99e0a-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="99e0a-104">Asegúrese de que tiene una suscripción que permita licencias de cliente, así como Office 365 Empresa o Empresa Premium, y [asegúrese de que el usuario tenga asignada una licencia](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="99e0a-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="99e0a-105">Asegúrese de que el usuario inicia sesión en Office con la misma cuenta a la que se ha asignado la licencia.</span><span class="sxs-lookup"><span data-stu-id="99e0a-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="99e0a-106">Consulte la [página de estado del servicio de Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver si hay problemas conocidos con el servicio.</span><span class="sxs-lookup"><span data-stu-id="99e0a-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="99e0a-107">Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no están bloqueando el acceso de las aplicaciones de Microsoft 365 a Internet.</span><span class="sxs-lookup"><span data-stu-id="99e0a-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="99e0a-108">Consulte [Intervalos de direcciones IP y URL de Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Intervalos de direcciones IP y direcciones URL de Office 365").</span><span class="sxs-lookup"><span data-stu-id="99e0a-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="99e0a-109">**Sugerencia** en equipos Windows, podemos diagnosticar y solucionar varios problemas comunes de inicio de sesión de Office.</span><span class="sxs-lookup"><span data-stu-id="99e0a-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="99e0a-110">Descargue y ejecute el **[Asistente de soporte y recuperación de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nuestra herramienta automatizada.</span><span class="sxs-lookup"><span data-stu-id="99e0a-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="99e0a-111">Haga lo siguiente para intentar solucionar el problema:</span><span class="sxs-lookup"><span data-stu-id="99e0a-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="99e0a-112">Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes.</span><span class="sxs-lookup"><span data-stu-id="99e0a-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="99e0a-113">[Elimine](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) y [reasigne](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) la licencia de Office y, después, [inicie sesión en Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.</span><span class="sxs-lookup"><span data-stu-id="99e0a-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="99e0a-114">Ejecute el [Solucionador de problemas de activación](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="99e0a-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="99e0a-115">Restablezca el estado de activación de Office</span><span class="sxs-lookup"><span data-stu-id="99e0a-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Restablezca el estado de activación de Office")
- [<span data-ttu-id="99e0a-116">Realice una reparación en línea de Office</span><span class="sxs-lookup"><span data-stu-id="99e0a-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="99e0a-117">Para ver más medidas de solución de problemas, vea:</span><span class="sxs-lookup"><span data-stu-id="99e0a-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="99e0a-118">Errores de activación y de producto sin licencia en Office</span><span class="sxs-lookup"><span data-stu-id="99e0a-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="99e0a-119">Error "Lo sentimos, no podemos conectarnos con su cuenta. Inténtelo de nuevo más tarde" al activar Office</span><span class="sxs-lookup"><span data-stu-id="99e0a-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)