---
title: Creación de una relación de organización para permitir que los usuarios colaboren con otra organización
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854042"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="a67e5-102">Creación de una relación de organización para permitir que los usuarios colaboren con otra organización</span><span class="sxs-lookup"><span data-stu-id="a67e5-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="a67e5-103">En el panel del Centro de administración de Microsoft 365, vaya a **Administración** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="a67e5-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="a67e5-104">Vaya a **Organización** > **Uso compartido**.</span><span class="sxs-lookup"><span data-stu-id="a67e5-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="a67e5-105">En **Uso compartido de la organización**, haga clic en **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="a67e5-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="a67e5-106">En el cuadro **Nombre de la relación** de **nueva relación de organización**, escriba un nombre descriptivo para la relación de organización.</span><span class="sxs-lookup"><span data-stu-id="a67e5-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="a67e5-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span><span class="sxs-lookup"><span data-stu-id="a67e5-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="a67e5-108">If you need to enter more than one domain, separate the domain names with a comma.</span><span class="sxs-lookup"><span data-stu-id="a67e5-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="a67e5-109">For example, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="a67e5-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="a67e5-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span><span class="sxs-lookup"><span data-stu-id="a67e5-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="a67e5-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span><span class="sxs-lookup"><span data-stu-id="a67e5-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="a67e5-112">Para configurar el nivel de acceso a la información de disponibilidad, seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="a67e5-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="a67e5-113">**Información de disponibilidad de calendario solo con hora**</span><span class="sxs-lookup"><span data-stu-id="a67e5-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="a67e5-114">**Disponibilidad de calendario con hora, asunto y ubicación**</span><span class="sxs-lookup"><span data-stu-id="a67e5-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="a67e5-115">Para especificar los usuarios que van a compartir la información de disponibilidad de calendario, seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="a67e5-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="a67e5-116">**Todos en su organización**</span><span class="sxs-lookup"><span data-stu-id="a67e5-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="a67e5-117">**Un grupo de seguridad especificado**</span><span class="sxs-lookup"><span data-stu-id="a67e5-117">**A specified security group**</span></span>  

<span data-ttu-id="a67e5-118">Haga clic en **Examinar** para elegir el grupo de seguridad de una lista y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="a67e5-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="a67e5-119">Haga clic en **guardar** para crear la relación de organización.</span><span class="sxs-lookup"><span data-stu-id="a67e5-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="a67e5-120">**Nota:** las configuraciones entre espacios empresariales no admiten contactos personales para búsqueda de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="a67e5-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="a67e5-121">Los contactos deben incluirse en la lista global de direcciones para que la búsqueda de disponibilidad funcione.</span><span class="sxs-lookup"><span data-stu-id="a67e5-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="a67e5-122">**Para comprender completamente este tema, lea:**</span><span class="sxs-lookup"><span data-stu-id="a67e5-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="a67e5-123">Crear una relación de organización en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a67e5-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="a67e5-124">Modificar una relación de organización en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a67e5-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="a67e5-125">Quitar una relación de organización en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a67e5-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
