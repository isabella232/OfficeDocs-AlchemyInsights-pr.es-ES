---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813777"
---
# <a name="error-attributevaluemustbeunique"></a>Error: AttributeValueMustBeUnique

El motivo más común del error AttributeValueMustBeUnique es que dos objetos con sourceanchor (inmutableId) diferentes tienen el mismo valor para los atributos ProxyAddresses y/o UserPrincipalName. Para corregir el error AttributeValueMustBeUnique:
  
1. Identifique los proxyAddresses duplicados, userPrincipalName u otro valor de atributo que está provocando el error. Identifique también qué dos (o más) objetos están implicados en el conflicto. El informe generado por Azure AD Connect Health para la sincronización puede ayudarle a identificar los dos objetos.
    
2. Identifique qué objeto debe seguir teniendo el valor duplicado y qué objeto no debe.
    
3. Quite el valor duplicado del objeto que NO debería tener ese valor. Tenga en cuenta que debe realizar el cambio en el directorio desde el que el objeto es de origen. En algunos casos, es posible que deba eliminar uno de los objetos en conflicto.
    
4. Si ha realizado el cambio en el AD local, deje que Azure AD Connect sincronice el cambio para que el error se solucione.
    

