---
title: Acceso a la suscripción
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773782"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="ff819-102">No se puede iniciar sesión en Azure debido a problemas en el explorador (el explorador se bloquea, sigue girando, no se carga, etc.).</span><span class="sxs-lookup"><span data-stu-id="ff819-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="ff819-103">Es posible que se vea afectado por una interrupción.</span><span class="sxs-lookup"><span data-stu-id="ff819-103">You might be impacted by an outage.</span></span> <span data-ttu-id="ff819-104">Compruebe si hay una interrupción continua: [Estado de Azure Health](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="ff819-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="ff819-105">Cierre sesión en todas las sesiones de Azure activas.</span><span class="sxs-lookup"><span data-stu-id="ff819-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="ff819-106">Inicie un modo en privado o incógnito de su explorador Web.</span><span class="sxs-lookup"><span data-stu-id="ff819-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="ff819-107">También puede intentar actualizar el explorador, usar otro explorador y eliminar las cookies de caché si no funciona.</span><span class="sxs-lookup"><span data-stu-id="ff819-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="ff819-108">Más información: [solución de problemas de inicio de sesión](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="ff819-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="ff819-109">**No se puede tener acceso a las suscripciones**</span><span class="sxs-lookup"><span data-stu-id="ff819-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="ff819-110">En [Azure portal](https://portal.azure.com/), asegúrese de que se selecciona el directorio de Azure correcto en la cuenta de la parte superior derecha.</span><span class="sxs-lookup"><span data-stu-id="ff819-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="ff819-111">En el [centro de cuentas de Azure](https://account.windowsazure.com/Subscriptions), asegúrese de que la cuenta usada sea el administrador de la cuenta.</span><span class="sxs-lookup"><span data-stu-id="ff819-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="ff819-112">Más información: [solucionar problemas no se encontraron suscripciones](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ff819-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="ff819-113">**No se puede obtener acceso al historial de facturación**</span><span class="sxs-lookup"><span data-stu-id="ff819-113">**Unable to access billing history**</span></span>

<span data-ttu-id="ff819-114">El administrador de la cuenta debe asegurarse de que el usuario que tiene acceso a la información de facturación se agrega a Azure Active Directory como usuario invitado: [Agregar o eliminar un nuevo usuario](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ff819-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff819-115">A continuación, el usuario debe tener un rol de administrador global: [asignar rol a los usuarios](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ff819-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff819-116">Registrar esto, al usuario se le puede conceder acceso a la facturación mediante directivas RBAC: [conceder acceso a la facturación](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ff819-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff819-117">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="ff819-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="ff819-118">No puedo iniciar sesión para administrar mi suscripción a Azure</span><span class="sxs-lookup"><span data-stu-id="ff819-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)