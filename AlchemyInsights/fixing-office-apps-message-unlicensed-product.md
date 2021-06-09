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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798697"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="87034-102">No se ha podido activar Office</span><span class="sxs-lookup"><span data-stu-id="87034-102">Unable to activate Office</span></span>

<span data-ttu-id="87034-103">**Nota**: Si usa una versión anterior de Windows (por ejemplo, Windows 7), asegúrese de que TLS 1.2 esté habilitado como predeterminado.</span><span class="sxs-lookup"><span data-stu-id="87034-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="87034-104">Para obtener más información, consulte [Actualizar para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="87034-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="87034-105">Compruebe el estado de la suscripción para ver si ha caducado.</span><span class="sxs-lookup"><span data-stu-id="87034-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="87034-106">Asegúrese de que tiene una suscripción que permita licencias de cliente, así como Office 365 Empresa o Empresa Premium, y [asegúrese de que el usuario tenga asignada una licencia](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="87034-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="87034-107">Asegúrese de que el usuario inicia sesión en Office con la misma cuenta a la que se ha asignado la licencia.</span><span class="sxs-lookup"><span data-stu-id="87034-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="87034-108">Consulte la [página de estado del servicio de Office 365](/office365/enterprise/view-service-health) para ver si hay problemas conocidos con el servicio.</span><span class="sxs-lookup"><span data-stu-id="87034-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="87034-p102">Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no bloquean el acceso de las aplicaciones de Microsoft 365 a Internet. Consulte [Intervalos de direcciones IP y URL de Office 365](/office365/enterprise/urls-and-ip-address-ranges "Intervalos de direcciones IP y direcciones URL de Office 365").</span><span class="sxs-lookup"><span data-stu-id="87034-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="87034-111">**Sugerencia** en equipos Windows, podemos diagnosticar y solucionar varios problemas comunes de inicio de sesión de Office.</span><span class="sxs-lookup"><span data-stu-id="87034-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="87034-112">Descargue y ejecute el **[Asistente de soporte y recuperación de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nuestra herramienta automatizada.</span><span class="sxs-lookup"><span data-stu-id="87034-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="87034-113">Haga lo siguiente para intentar solucionar el problema:</span><span class="sxs-lookup"><span data-stu-id="87034-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="87034-114">Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes.</span><span class="sxs-lookup"><span data-stu-id="87034-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="87034-115">[Elimine](/microsoft-365/admin/manage/remove-licenses-from-users) y [reasigne](/microsoft-365/admin/manage/assign-licenses-to-users) la licencia de Office y, después, [inicie sesión en Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.</span><span class="sxs-lookup"><span data-stu-id="87034-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="87034-116">Ejecute el [Solucionador de problemas de activación](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="87034-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="87034-117">Restablezca el estado de activación de Office</span><span class="sxs-lookup"><span data-stu-id="87034-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Restablezca el estado de activación de Office")
- [<span data-ttu-id="87034-118">Realice una reparación en línea de Office</span><span class="sxs-lookup"><span data-stu-id="87034-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="87034-119">Para ver más medidas de solución de problemas, vea:</span><span class="sxs-lookup"><span data-stu-id="87034-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="87034-120">Errores de activación y de producto sin licencia en Office</span><span class="sxs-lookup"><span data-stu-id="87034-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="87034-121">Error "Lo sentimos, no podemos conectarnos con su cuenta. Inténtelo de nuevo más tarde" al activar Office</span><span class="sxs-lookup"><span data-stu-id="87034-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)