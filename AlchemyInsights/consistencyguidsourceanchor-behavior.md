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
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamiento de ConsistencyGuid / sourceAnchor

Azure AD Connect (versión 1.1.524.0 y posterior) ahora facilita el uso de msDS-ConsistencyGuid como atributo sourceAnchor. Al usar esta característica, Azure AD Connect configura automáticamente las reglas de sincronización para:
  
- Use msDS-ConsistencyGuid como atributo sourceAnchor para objetos User. ObjectGUID se usa para otros tipos de objeto.
    
- Para cualquier objeto de usuario de AD local determinado cuyo atributo msDS-ConsistencyGuid no esté rellenado, Azure AD Connect escribe su valor objectGUID de nuevo en el atributo msDS-ConsistencyGuid en Active Directory local. Después de rellenar el atributo msDS-ConsistencyGuid, Azure AD Connect exporta el objeto a Azure AD.
    
 **Nota:** Una vez que un objeto de AD local se importa en Azure AD Connect (es decir, se importa en el espacio de AD Connector y se proyecta en el Metaverso), ya no puede cambiar su valor sourceAnchor. Para especificar el valor sourceAnchor para un objeto de AD local determinado, configure su atributo msDS-ConsistencyGuid antes de importarlo a Azure AD Connect. 
  
Para obtener más información sobre SourceAnchor y ConsistencyGuid, consulte: [Azure AD Connect: Conceptos de diseño](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

