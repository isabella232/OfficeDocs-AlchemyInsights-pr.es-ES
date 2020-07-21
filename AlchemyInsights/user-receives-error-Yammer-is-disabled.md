---
title: El usuario recibe el error AADSTS7000112 Yammer is disabled
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157335"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="51056-102">El usuario recibe el error AADSTS7000112 Yammer is disabled</span><span class="sxs-lookup"><span data-stu-id="51056-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="51056-103">Si recibe el error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", hay un problema con la entidad de servicio en Azure AD.</span><span class="sxs-lookup"><span data-stu-id="51056-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="51056-104">Es posible que el administrador haya deshabilitado la entidad de servicio para bloquear el acceso a Yammer.</span><span class="sxs-lookup"><span data-stu-id="51056-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="51056-105">No se recomienda deshabilitar la entidad de servicio, porque puede provocar problemas adicionales.</span><span class="sxs-lookup"><span data-stu-id="51056-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="51056-106">Para obtener más información sobre el método admitido para bloquear el acceso de los usuarios a Yammer, vea [Desactivar el acceso de usuarios de Microsoft 365 a Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="51056-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="51056-107">Para corregir este problema en Azure Portal y restaurar el acceso de los usuarios a Yammer, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="51056-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="51056-108">Abra la página de Azure Active Directory y seleccione **Aplicaciones empresariales** en **Administrar** en el panel de navegación izquierdo.</span><span class="sxs-lookup"><span data-stu-id="51056-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="51056-109">Escriba **Yammer de Office 365** en el cuadro de búsqueda y seleccione el nombre de la aplicación para abrir configuración.</span><span class="sxs-lookup"><span data-stu-id="51056-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="51056-110">Seleccione **Propiedades** en **Administrar** en el panel de navegación izquierdo.</span><span class="sxs-lookup"><span data-stu-id="51056-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="51056-111">Establezca el valor **¿Habilitado para que los usuarios inicien sesión?** en **Sí** y, después, seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="51056-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="51056-112">Vuelva a iniciar sesión en Yammer.</span><span class="sxs-lookup"><span data-stu-id="51056-112">Sign in to Yammer again.</span></span> <span data-ttu-id="51056-113">Es posible que deba borrar las cookies.</span><span class="sxs-lookup"><span data-stu-id="51056-113">You might need to clear cookies.</span></span>

<span data-ttu-id="51056-114">También puede ejecutar los comandos de PowerShell para establecer el valor.</span><span class="sxs-lookup"><span data-stu-id="51056-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="51056-115">Para obtener más información, vea ["Lo sentimos, pero estamos teniendo problemas para iniciar su sesión" al hacer clic en el icono de Yammer en Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="51056-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 