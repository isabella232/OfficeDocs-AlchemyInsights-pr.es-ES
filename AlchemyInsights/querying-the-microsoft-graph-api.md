---
title: Consulta de la API de Microsoft Graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950779"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="d647e-102">Consulta de la API de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="d647e-103">Este tema también puede aplicarse a los desarrolladores que aún usan la API de Graph de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d647e-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="d647e-104">Sin embargo, se **recomienda usar** Microsoft Graph para todos los escenarios de administración de acceso, identidad y directorio.</span><span class="sxs-lookup"><span data-stu-id="d647e-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="d647e-105">**Problemas de autenticación o autorización**</span><span class="sxs-lookup"><span data-stu-id="d647e-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="d647e-106">Si su aplicación no puede adquirir **tokens** para llamar a Microsoft Graph, elija Problema con la obtención de una categoría de Microsoft Graph de token de acceso **(autenticación)** para obtener ayuda y soporte técnico más específicos en este tema.</span><span class="sxs-lookup"><span data-stu-id="d647e-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="d647e-107">Si la aplicación recibe errores de autorización **401 o 403** al llamar a Microsoft Graph, seleccione la categoría obtener un error de acceso denegado **(Autorización)** de la API de Microsoft Graph para obtener ayuda y soporte técnico más específicos en este tema.</span><span class="sxs-lookup"><span data-stu-id="d647e-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="d647e-108">**Quiero usar Microsoft Graph, pero no sé por dónde empezar**</span><span class="sxs-lookup"><span data-stu-id="d647e-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="d647e-109">Para obtener más información sobre Microsoft Graph, vea:</span><span class="sxs-lookup"><span data-stu-id="d647e-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="d647e-110">Información general de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="d647e-111">Información general sobre la administración de identidades y acceso en Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="d647e-112">Introducción a la creación de aplicaciones de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="d647e-113">**Explorador de Microsoft Graph:** probar las API de Microsoft Graph en el espacio empresarial o en un inquilino de demostración</span><span class="sxs-lookup"><span data-stu-id="d647e-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="d647e-114">**Quiero usar Microsoft Graph, pero ¿es compatible con las API de directorio v1.0 que necesito?**</span><span class="sxs-lookup"><span data-stu-id="d647e-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="d647e-115">Microsoft Graph es la API recomendada para la administración de directorios, identidades y acceso.</span><span class="sxs-lookup"><span data-stu-id="d647e-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="d647e-116">Sin embargo, todavía hay algunas diferencias entre lo que es posible en Azure AD Graph y Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d647e-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="d647e-117">Revise los siguientes artículos, que resaltan las diferencias más recientes para ayudarle en su elección:</span><span class="sxs-lookup"><span data-stu-id="d647e-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="d647e-118">Diferencias de tipo de recurso entre Azure AD Graph y Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="d647e-119">Diferencias de propiedades entre Azure AD Graph y Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="d647e-120">Diferencias de métodos entre Azure AD y Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="d647e-121">**Cuando se consulta el *objeto de* usuario, faltan muchas de sus propiedades**</span><span class="sxs-lookup"><span data-stu-id="d647e-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="d647e-122">`GET https://graph.microsoft.com/v1.0/users` solo devuelve 11 propiedades, ya que Microsoft Graph selecciona automáticamente un conjunto predeterminado de propiedades *de* usuario para devolver.</span><span class="sxs-lookup"><span data-stu-id="d647e-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="d647e-123">Si necesita *otras propiedades de* usuario, use $select para seleccionar las propiedades que necesita la aplicación.</span><span class="sxs-lookup"><span data-stu-id="d647e-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="d647e-124">Pruébalo primero **en el Explorador de Microsoft Graph.**</span><span class="sxs-lookup"><span data-stu-id="d647e-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="d647e-125">**Algunos valores de propiedad de usuario *son nulos* aunque sé que están establecidos**</span><span class="sxs-lookup"><span data-stu-id="d647e-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="d647e-126">La explicación más probable es que a la aplicación se le había concedido el *permiso User.ReadBasic.All.*</span><span class="sxs-lookup"><span data-stu-id="d647e-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="d647e-127">Esto permite a la aplicación leer un conjunto limitado de propiedades de usuario, devolviendo todas las demás propiedades como nulas incluso si se han establecido anteriormente.</span><span class="sxs-lookup"><span data-stu-id="d647e-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="d647e-128">En su lugar, intente conceder el *permiso User.Read.All* a la aplicación.</span><span class="sxs-lookup"><span data-stu-id="d647e-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="d647e-129">Para obtener más información, vea [Permisos de usuario de Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="d647e-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="d647e-130">**Tengo problemas para usar parámetros de consulta de OData para filtrar datos en mis solicitudes**</span><span class="sxs-lookup"><span data-stu-id="d647e-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="d647e-131">Aunque Microsoft Graph admite una amplia gama de parámetros de consulta de OData, muchos de esos parámetros no son totalmente compatibles con los servicios de directorio (recursos que heredan de *directoryObject)* en Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d647e-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="d647e-132">Las mismas limitaciones que estaban presentes en Azure AD Graph persisten en su mayoría en Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="d647e-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="d647e-133">**No se** admite: $count, $search y $filter *valores null* o *no null*</span><span class="sxs-lookup"><span data-stu-id="d647e-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="d647e-134">**No se admite:**$filter en determinadas propiedades (vea temas de recursos sobre qué propiedades se pueden filtrar)</span><span class="sxs-lookup"><span data-stu-id="d647e-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="d647e-135">**No se admite:** paginación, filtrado y ordenación al mismo tiempo</span><span class="sxs-lookup"><span data-stu-id="d647e-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="d647e-136">**No se admite:** filtrado en una relación.</span><span class="sxs-lookup"><span data-stu-id="d647e-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="d647e-137">Por ejemplo: busque todos los miembros del grupo de ingeniería que están en el Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="d647e-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="d647e-138">**Compatibilidad parcial:**$orderby *usuario* (solo displayName y userPrincipalName) y *grupo*</span><span class="sxs-lookup"><span data-stu-id="d647e-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="d647e-139">**Compatibilidad parcial:**$filter (solo admite compatibilidad *con eq*, *startswith* o *,* o *,* y , y limitado cualquier *),*$expand (expandir las relaciones de un solo objeto devuelve todas las relaciones, pero expandir una colección de relaciones de objetos es limitado)</span><span class="sxs-lookup"><span data-stu-id="d647e-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="d647e-140">Para obtener más información, vea [Personalizar las respuestas con parámetros de consulta.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="d647e-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="d647e-141">**The API I'm calling doesn't work- where can I do more testing?**</span><span class="sxs-lookup"><span data-stu-id="d647e-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="d647e-142">**Explorador de Microsoft Graph:** pruebe las API de Microsoft Graph en su espacio empresarial o en un espacio empresarial de demostración y consulte también las consultas de ejemplo **en** el Explorador de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d647e-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="d647e-143">**Cuando se consultan datos, parece que se obtiene un conjunto de datos incompleto**</span><span class="sxs-lookup"><span data-stu-id="d647e-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="d647e-144">Si está consultando una colección (como los *usuarios),* Microsoft Graph usa límites de página del lado servidor para que los resultados siempre se devuelvan con un tamaño de página predeterminado.</span><span class="sxs-lookup"><span data-stu-id="d647e-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="d647e-145">La aplicación siempre debe esperar pasar por las colecciones devueltas desde el servicio.</span><span class="sxs-lookup"><span data-stu-id="d647e-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="d647e-146">Para obtener más información, vea:</span><span class="sxs-lookup"><span data-stu-id="d647e-146">For more information, see:</span></span>

- [<span data-ttu-id="d647e-147">Procedimientos recomendados de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="d647e-148">Paginación de los datos de Microsoft Graph en la aplicación</span><span class="sxs-lookup"><span data-stu-id="d647e-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="d647e-149">**Mi aplicación es demasiado lenta y también se está limitando. ¿Qué mejoras puedo realizar?**</span><span class="sxs-lookup"><span data-stu-id="d647e-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="d647e-150">Dependiendo de su escenario, hay una variedad de opciones diferentes a su disposición para que la aplicación sea más performant y, en algunos casos, menos propensa a que el servicio las limite (cuando está realizando demasiadas llamadas).</span><span class="sxs-lookup"><span data-stu-id="d647e-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="d647e-151">Para más información, vea:</span><span class="sxs-lookup"><span data-stu-id="d647e-151">To learn more, see:</span></span>

- [<span data-ttu-id="d647e-152">Procedimientos recomendados de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="d647e-153">Solicitudes de procesamiento por lotes</span><span class="sxs-lookup"><span data-stu-id="d647e-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="d647e-154">Seguimiento de cambios a través de la consulta delta</span><span class="sxs-lookup"><span data-stu-id="d647e-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="d647e-155">Recibir notificaciones de cambios a través de webhooks</span><span class="sxs-lookup"><span data-stu-id="d647e-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="d647e-156">Guía de limitación</span><span class="sxs-lookup"><span data-stu-id="d647e-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="d647e-157">**¿Dónde puedo encontrar más información sobre errores y problemas conocidos?**</span><span class="sxs-lookup"><span data-stu-id="d647e-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="d647e-158">Información de respuesta de error de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="d647e-159">Problemas conocidos de Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d647e-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="d647e-160">**¿Dónde puedo comprobar el estado de disponibilidad y conectividad del servicio?**</span><span class="sxs-lookup"><span data-stu-id="d647e-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="d647e-161">La disponibilidad del servicio y la conectividad de los servicios subyacentes a los que se puede tener acceso a través de Microsoft Graph pueden afectar a la disponibilidad general y al rendimiento de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d647e-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="d647e-162">Para el estado del servicio de Azure Active Directory, compruebe el estado de seguridad **+ servicios** de identidad que aparecen en la página de estado [de Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="d647e-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="d647e-163">Para los servicios de Office que contribuyen a Microsoft Graph, compruebe el estado de los servicios enumerados en el Panel de estado del servicio [de Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="d647e-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
