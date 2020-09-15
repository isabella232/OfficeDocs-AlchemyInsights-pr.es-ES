---
title: Creación de una relación de organización para permitir que los usuarios colaboren con otra organización
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712750"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="8d2ae-102">Creación de una relación de organización para permitir que los usuarios colaboren con otra organización</span><span class="sxs-lookup"><span data-stu-id="8d2ae-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="8d2ae-103">En el panel del Centro de administración de Microsoft 365, vaya a **Administración** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="8d2ae-104">Vaya a **Organización** > **Uso compartido**.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="8d2ae-105">En **Uso compartido de la organización**, haga clic en **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="8d2ae-106">En el cuadro **Nombre de la relación** de **nueva relación de organización**, escriba un nombre descriptivo para la relación de organización.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="8d2ae-p101">En el cuadro **Dominios para compartir**, escriba el dominio para la organización externa de Office 365 o Exchange local a la que desea permitir que vea sus calendarios. Si necesita escribir más de un dominio, separe los nombres de dominio con una coma. Por ejemplo, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-p101">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars. If you need to enter more than one domain, separate the domain names with a comma. For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="8d2ae-p102">Active la casilla **Habilitar el uso compartido de la información de disponibilidad de calendario** para activar el uso compartido de calendario con los dominios que especifique. Establezca el nivel de uso compartido de la información de disponibilidad de calendario y defina qué usuarios pueden compartir esta información.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="8d2ae-112">Para configurar el nivel de acceso a la información de disponibilidad, seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="8d2ae-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="8d2ae-113">**Información de disponibilidad de calendario solo con hora**</span><span class="sxs-lookup"><span data-stu-id="8d2ae-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="8d2ae-114">**Disponibilidad de calendario con hora, asunto y ubicación**</span><span class="sxs-lookup"><span data-stu-id="8d2ae-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="8d2ae-115">Para especificar los usuarios que van a compartir la información de disponibilidad de calendario, seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="8d2ae-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="8d2ae-116">**Todos en su organización**</span><span class="sxs-lookup"><span data-stu-id="8d2ae-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="8d2ae-117">**Un grupo de seguridad especificado**</span><span class="sxs-lookup"><span data-stu-id="8d2ae-117">**A specified security group**</span></span>  

<span data-ttu-id="8d2ae-118">Haga clic en **Examinar** para elegir el grupo de seguridad de una lista y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="8d2ae-119">Haga clic en **guardar** para crear la relación de organización.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="8d2ae-120">**Nota:** las configuraciones entre espacios empresariales no admiten contactos personales para búsqueda de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="8d2ae-121">Los contactos deben incluirse en la lista global de direcciones para que la búsqueda de disponibilidad funcione.</span><span class="sxs-lookup"><span data-stu-id="8d2ae-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="8d2ae-122">**Para comprender completamente este tema, lea:**</span><span class="sxs-lookup"><span data-stu-id="8d2ae-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="8d2ae-123">Crear una relación de organización en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="8d2ae-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="8d2ae-124">Modificar una relación de organización en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="8d2ae-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="8d2ae-125">Quitar una relación de organización en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="8d2ae-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
