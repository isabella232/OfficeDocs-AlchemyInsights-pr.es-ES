---
title: Problemas con la concesión de licencias de Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657293"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="9e8bd-102">Problemas con la concesión de licencias de Yammer</span><span class="sxs-lookup"><span data-stu-id="9e8bd-102">Yammer licensing issues</span></span>

<span data-ttu-id="9e8bd-103">Todos los usuarios deben tener una licencia para usar el servicio de Yammer Enterprise, pero, de manera predeterminada, Yammer no necesita que los usuarios tengan una licencia para obtener acceso al servicio.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="9e8bd-104">Cuando un administrador cambia la configuración para bloquear a los usuarios de Microsoft 365 sin licencias de Yammer, los usuarios a los que no se les ha asignado una licencia de Yammer Enterprise no pueden obtener acceso al servicio de Yammer.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="9e8bd-105">Para obtener más información, vea [Administrar licencias de usuario de Yammer en Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9e8bd-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="9e8bd-106">Cuando se eliminan las licencias de los usuarios, ya no se muestra el icono de Yammer y otros servicios pueden usar la eliminación de la licencia para ocultar características.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="9e8bd-107">En otros casos, es posible que sigan apareciendo las características, pero que requieran una asignación de licencias para funcionar.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="9e8bd-108">**No se actualiza la licencia del usuario**</span><span class="sxs-lookup"><span data-stu-id="9e8bd-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="9e8bd-109">En ocasiones, se asigna una licencia a un usuario, pero sigue sin poder tener acceso a Yammer.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="9e8bd-110">Es probable que se produzcan retrasos cuando se está realizando una asignación masiva de licencias.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="9e8bd-111">Es posible que los usuarios de Yammer no se actualicen en el mismo orden en que se cambiaron las licencias en Azure AD porque el sistema se ejecuta de forma asincrónica.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="9e8bd-112">Espere 24 horas antes de abrir un caso de soporte técnico para informar de problemas de sincronización de licencias.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="9e8bd-113">**Asignación masiva de licencias**</span><span class="sxs-lookup"><span data-stu-id="9e8bd-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="9e8bd-114">Las licencias se pueden asignar mediante el centro de administración o mediante scripts de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="9e8bd-115">Para obtener más información, vea [Asignar licencias a los usuarios](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) y [Asignar licencias a cuentas de usuario con PowerShell de Office 365](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="9e8bd-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="9e8bd-116">El soporte técnico de Microsoft no proporciona asistencia para la creación de scripts, pero está disponible documentación sobre la asignación de licencias de Yammer.</span><span class="sxs-lookup"><span data-stu-id="9e8bd-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="9e8bd-117">Para obtener más información, vea [Administración de licencias de Yammer mediante Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="9e8bd-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>