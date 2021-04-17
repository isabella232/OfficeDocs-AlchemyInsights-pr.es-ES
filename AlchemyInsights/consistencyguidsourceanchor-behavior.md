---
title: Comportamiento de ConsistencyGuid / sourceAnchor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817009"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9649c-102">Comportamiento de ConsistencyGuid / sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="9649c-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9649c-103">Azure AD Connect (versión 1.1.524.0 y posterior) ahora facilita el uso de msDS-ConsistencyGuid como atributo sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9649c-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9649c-104">Al usar esta característica, Azure AD Connect configura automáticamente las reglas de sincronización para:</span><span class="sxs-lookup"><span data-stu-id="9649c-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9649c-105">Use msDS-ConsistencyGuid como atributo sourceAnchor para objetos User.</span><span class="sxs-lookup"><span data-stu-id="9649c-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9649c-106">ObjectGUID se usa para otros tipos de objeto.</span><span class="sxs-lookup"><span data-stu-id="9649c-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9649c-107">Para cualquier objeto de usuario de AD local determinado cuyo atributo msDS-ConsistencyGuid no esté rellenado, Azure AD Connect escribe su valor objectGUID de nuevo en el atributo msDS-ConsistencyGuid en Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="9649c-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9649c-108">Después de rellenar el atributo msDS-ConsistencyGuid, Azure AD Connect exporta el objeto a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9649c-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9649c-109">**Nota:** Una vez que un objeto de AD local se importa en Azure AD Connect (es decir, se importa en el espacio de AD Connector y se proyecta en el Metaverso), ya no puede cambiar su valor sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9649c-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9649c-110">Para especificar el valor sourceAnchor para un objeto de AD local determinado, configure su atributo msDS-ConsistencyGuid antes de importarlo a Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9649c-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9649c-111">Para obtener más información sobre SourceAnchor y ConsistencyGuid, consulte: [Azure AD Connect: Conceptos de diseño](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9649c-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

