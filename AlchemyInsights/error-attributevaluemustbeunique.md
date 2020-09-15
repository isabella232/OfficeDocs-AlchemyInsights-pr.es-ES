---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709168"
---
# <a name="error-attributevaluemustbeunique"></a>Error: AttributeValueMustBeUnique

La causa más común del error AttributeValueMustBeUnique son dos objetos con diferentes SourceAnchor (immutableId) que tienen el mismo valor para los atributos ProxyAddresses y UserPrincipalName. Para corregir el error AttributeValueMustBeUnique:
  
1. Identifique el valor de atributo proxyAddresses, userPrincipalName u otro atributo duplicado que está causando el error. Identifique también qué dos (o más) objetos participan en el conflicto. El informe generado por Azure AD Connect Health for Sync puede ayudarle a identificar los dos objetos.
    
2. Identifique qué objeto debe seguir teniendo el valor duplicado y qué objeto no debería.
    
3. Quite el valor duplicado del objeto que no debe tener ese valor. Tenga en cuenta que debe realizar el cambio en el directorio desde el que se origina el objeto. En algunos casos, es posible que deba eliminar uno de los objetos en conflicto.
    
4. Si realizó el cambio en el anuncio local, deje que Azure AD Connect sincronice el cambio para que se corrija el error.
    

