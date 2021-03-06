---
title: Problema con el atributo y el filtro de alcance
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430780"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="25beb-102">Problema con el atributo y el filtro de alcance</span><span class="sxs-lookup"><span data-stu-id="25beb-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="25beb-103">**Problema con valores UPN en conflicto**</span><span class="sxs-lookup"><span data-stu-id="25beb-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="25beb-104">El aprovisionamiento de usuarios de Workday para AD muestra un mensaje de error **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="25beb-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="25beb-105">La operación falló porque el valor UPN proporcionado para la adición / modificación no es único en todo el bosque.</span><span class="sxs-lookup"><span data-stu-id="25beb-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="25beb-106">Detalles del error: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="25beb-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="25beb-107">El valor **userPrincipalName** que el conector del Workday intenta asignar al crear la cuenta de usuario de AD ya existe en el dominio objetivo de AD.</span><span class="sxs-lookup"><span data-stu-id="25beb-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="25beb-108">Esto implica que o bien (1) el usuario ya existe y la comprobación de ID coincidente falló para el usuario o que (2) la regla de generación de UPN generó un valor conflictivo.</span><span class="sxs-lookup"><span data-stu-id="25beb-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="25beb-109">Aquí se muestran los pasos de resolución sugeridos:</span><span class="sxs-lookup"><span data-stu-id="25beb-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="25beb-110">Si el usuario ya existe y la comprobación de ID coincidente no pudo vincular la cuenta de Workday a la cuenta de Active Directory, verifique si el atributo de ID coincidente (normalmente **employeeID**), tanto en Workday como en AD, tiene una coincidencia exacta.</span><span class="sxs-lookup"><span data-stu-id="25beb-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="25beb-111">Si no tienen una coincidencia, es un problema de datos que debe solucionarse.</span><span class="sxs-lookup"><span data-stu-id="25beb-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="25beb-112">Por ejemplo, si el EmployeeID en Workday es 001052 y en AD es 1052, el motor de aprovisionamiento no podrá vincular las dos cuentas e intentará crear un usuario que ya exista.</span><span class="sxs-lookup"><span data-stu-id="25beb-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="25beb-113">En este caso, la solución consiste en cambiar el valor de **EmployeeID** en AD para incluir los ceros iniciales para que sea 001052.</span><span class="sxs-lookup"><span data-stu-id="25beb-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="25beb-114">Si la expresión generadora de UPN no genera un valor único, considere usar la función de reduplicado **SelectUniqueValue** para generar un valor único cada vez.</span><span class="sxs-lookup"><span data-stu-id="25beb-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="25beb-115">**El Workday para el aprovisionamiento de usuarios de AD no establece el valor de atributo de administrador para la cuenta de usuario de AD**</span><span class="sxs-lookup"><span data-stu-id="25beb-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="25beb-116">El trabajo del Workday para el aprovisionamiento de usuarios de AD no establece el valor de atributo de **administrador** para las cuentas de usuario de AD.</span><span class="sxs-lookup"><span data-stu-id="25beb-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="25beb-117">Hay dos escenarios posibles cuando se observa este comportamiento:</span><span class="sxs-lookup"><span data-stu-id="25beb-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="25beb-118">El administrador en el Workday no se puede resolver en una cuenta de usuario de AD correspondiente porque el administrador no es de su ámbito.</span><span class="sxs-lookup"><span data-stu-id="25beb-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="25beb-119">En un escenario de **múltiples dominios de AD**, el administrador del Workday no está presente en el mismo dominio que el usuario.</span><span class="sxs-lookup"><span data-stu-id="25beb-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="25beb-120">Pruebe estos pasos para solucionar el problema:</span><span class="sxs-lookup"><span data-stu-id="25beb-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="25beb-121">Si ha definido filtros del ámbito, primero verifique si el administrador está en su ámbito y si cumple con la cláusula del ámbito.</span><span class="sxs-lookup"><span data-stu-id="25beb-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="25beb-122">Si el administrador no satisface el filtro del ámbito, cámbielo para que el administrador también esté dentro del ámbito de la operación de aprovisionamiento.</span><span class="sxs-lookup"><span data-stu-id="25beb-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="25beb-123">Si tiene varios dominios de AD, el conector tiene una limitación conocida de incapacidad para resolver las referencias de administrador entre dominios.</span><span class="sxs-lookup"><span data-stu-id="25beb-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="25beb-124">Para obtener más información sobre cómo configurar Workday para el aprovisionamiento automatizado, vea [Tutorial: configurar Workday para el aprovisionamiento automático de usuarios](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="25beb-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













