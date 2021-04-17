---
title: Creación de una directiva de uso compartido para permitir que los usuarios compartan sus calendarios con personas fuera de su organización
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816289"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="c86a4-102">Creación de una directiva de uso compartido para permitir que los usuarios compartan sus calendarios con personas fuera de su organización</span><span class="sxs-lookup"><span data-stu-id="c86a4-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="c86a4-103">En el panel del Centro de administración de Microsoft 365, vaya a **Administración** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c86a4-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="c86a4-104">Vaya a **Organización** > **Uso compartido**.</span><span class="sxs-lookup"><span data-stu-id="c86a4-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="c86a4-105">En la vista de lista, en **Uso compartido individual**, haga clic en **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="c86a4-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="c86a4-106">En **Nueva directiva compartida**, escriba un nombre descriptivo para la directiva de uso compartido en el cuadro **Nombre de la directiva**.</span><span class="sxs-lookup"><span data-stu-id="c86a4-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="c86a4-107">Haga clic en **Agregar** para definir las reglas de uso compartido de la directiva.</span><span class="sxs-lookup"><span data-stu-id="c86a4-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="c86a4-108">En **regla de uso compartido**, seleccione una de las siguientes opciones para especificar los dominios con los que desea compartir:</span><span class="sxs-lookup"><span data-stu-id="c86a4-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="c86a4-109">**Compartir con todos los dominios**</span><span class="sxs-lookup"><span data-stu-id="c86a4-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="c86a4-110">**Compartir con un dominio específico**</span><span class="sxs-lookup"><span data-stu-id="c86a4-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="c86a4-p101">Si selecciona **Compartir con un dominio específico**, escriba el dominio con el que desea compartir. Si necesita indicar más de un dominio para esta directiva de uso compartido, guarde la configuración del primer dominio y, después, cambie las reglas de uso compartido para agregar más dominios.</span><span class="sxs-lookup"><span data-stu-id="c86a4-p101">If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="c86a4-113">Para especificar la información que se va a poder compartir, active la casilla **Compartir la carpeta de calendario** y, a continuación, seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="c86a4-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="c86a4-114">**Información de disponibilidad de calendario solo con hora**</span><span class="sxs-lookup"><span data-stu-id="c86a4-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="c86a4-115">**Información de disponibilidad de calendario con hora, asunto y ubicación**</span><span class="sxs-lookup"><span data-stu-id="c86a4-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="c86a4-116">**Toda la información de citas de calendarios, incluidas la hora, el asunto, la ubicación y el título**</span><span class="sxs-lookup"><span data-stu-id="c86a4-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="c86a4-117">Haga clic en **guardar** para configurar las reglas de la directiva de uso compartido.</span><span class="sxs-lookup"><span data-stu-id="c86a4-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="c86a4-118">Si quiere establecer esta directiva de uso compartido como nueva directiva predeterminada para todos los usuarios de la organización, active la casilla **Hacer que esta sea mi directiva de uso compartido predeterminada**.</span><span class="sxs-lookup"><span data-stu-id="c86a4-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="c86a4-119">Haga clic en **Guardar** para crear la directiva de uso compartido.</span><span class="sxs-lookup"><span data-stu-id="c86a4-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="c86a4-120">**Para comprender completamente este tema, lea:**</span><span class="sxs-lookup"><span data-stu-id="c86a4-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="c86a4-121">Crear una directiva de uso compartido en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c86a4-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="c86a4-122">Aplicar una directiva de uso compartido a buzones de correo en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c86a4-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="c86a4-123">Modificar, deshabilitar o quitar una directiva de uso compartido en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c86a4-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)