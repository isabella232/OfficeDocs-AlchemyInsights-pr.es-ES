---
title: Problema con un solo usuario
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428829"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="b52b2-102">Problema con un solo usuario</span><span class="sxs-lookup"><span data-stu-id="b52b2-102">Problem with single user</span></span>

- <span data-ttu-id="b52b2-103">Es posible que el usuario no se haya aprovisionado porque el servicio aún no ha tenido la oportunidad de evaluarlo.</span><span class="sxs-lookup"><span data-stu-id="b52b2-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="b52b2-104">Revise las instrucciones sobre cuánto tarda el aprovisionamiento, así como la barra de progreso de la página de configuración de aprovisionamiento.</span><span class="sxs-lookup"><span data-stu-id="b52b2-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="b52b2-105">Si el estado estable especificado en la sección de detalles adicionales es anterior a la fecha en que se creó/actualizó o eliminó el usuario, significa que aún no hemos evaluado al usuario.</span><span class="sxs-lookup"><span data-stu-id="b52b2-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="b52b2-106">En este escenario, lo mejor que se puede hacer es esperar a que finalice el servicio de aprovisionamiento.</span><span class="sxs-lookup"><span data-stu-id="b52b2-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="b52b2-107">Tenga en cuenta que nuestro servicio solo tiene en cuenta los cambios realizados en un usuario en el sistema de origen (HR en la nube).</span><span class="sxs-lookup"><span data-stu-id="b52b2-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="b52b2-108">Debe haber un cambio válido en el sistema de origen para que Azure AD detecte el cambio y lo fluya a Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b52b2-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="b52b2-109">El servicio de aprovisionamiento evaluó al usuario y determinó que no debe aprovisionarse:</span><span class="sxs-lookup"><span data-stu-id="b52b2-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="b52b2-110">Si ha establecido un filtro de ámbito basado en atributos, asegúrese de que el usuario cumple los criterios especificados.</span><span class="sxs-lookup"><span data-stu-id="b52b2-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="b52b2-111">Si los usuarios ya existen en el sistema de destino y el estado del usuario en la coincidencia de origen y destino, no realizaremos ninguna acción adicional.</span><span class="sxs-lookup"><span data-stu-id="b52b2-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="b52b2-112">El servicio de aprovisionamiento intentó aprovisionar al usuario y falló.</span><span class="sxs-lookup"><span data-stu-id="b52b2-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="b52b2-113">Para estos escenarios, revise la pestaña solución de problemas y recomendaciones de los registros de aprovisionamiento:</span><span class="sxs-lookup"><span data-stu-id="b52b2-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="b52b2-114">Es posible que falte un atributo obligatorio en el usuario en Active Directory local o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b52b2-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="b52b2-115">Por ejemplo, las reglas de generación userPrincipalName o sAMAccountName no están generando el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="b52b2-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="b52b2-116">El atributo de coincidencia (normalmente employeeId) no se resuelve para un usuario único en Active Directory local o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b52b2-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="b52b2-117">Por ejemplo, hay dos usuarios con el mismo employeeId en AD y el servicio devuelve un código de error que indica entradas de destino duplicadas para la misma entrada de origen.</span><span class="sxs-lookup"><span data-stu-id="b52b2-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="b52b2-118">Para revisar los registros de un solo usuario y grupos, vea [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="b52b2-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
