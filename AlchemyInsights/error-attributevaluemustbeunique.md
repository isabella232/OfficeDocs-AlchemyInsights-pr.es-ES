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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002140"
---
# <a name="error-attributevaluemustbeunique"></a>Error: AttributeValueMustBeUnique

El motivo más común del error AttributeValueMustBeUnique es que dos objetos con sourceanchor (inmutableId) diferentes tienen el mismo valor para los atributos ProxyAddresses y/o UserPrincipalName. Para corregir el error AttributeValueMustBeUnique:
  
1. Identifique los proxyAddresses duplicados, userPrincipalName u otro valor de atributo que está provocando el error. Identifique también qué dos (o más) objetos están implicados en el conflicto. El informe generado por Azure AD Conectar Health para la sincronización puede ayudarle a identificar los dos objetos.
    
2. Identifique qué objeto debe seguir teniendo el valor duplicado y qué objeto no debe.
    
3. Quite el valor duplicado del objeto que NO debería tener ese valor. Tenga en cuenta que debe realizar el cambio en el directorio desde el que el objeto es de origen. En algunos casos, es posible que deba eliminar uno de los objetos en conflicto.
    
4. Si realizó el cambio en el AD local, deje que Azure AD Conectar sincronice el cambio para que el error se corrigió.
    

