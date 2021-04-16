---
title: Verify your domain
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
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771008"
---
# <a name="verify-your-domain"></a>Verify your domain

 **Es probable que el registro no se haya actualizado en Internet.**
  
Normalmente, solo nos lleva unos minutos poder ver el nuevo registro, pero de vez en cuando puede tardar unas horas. 
  
- Si ya ha esperado tanto tiempo, compruebe que ha copiado y pegado el valor exacto en el registro de comprobación TXT en el host DNS. Uno de los problemas habituales es no incluir la parte de "MS=" del registro. ¡También la necesitamos!

- En algunos hosts DNS, tiene que llevar a cabo un paso adicional para guardar el archivo de zona (donde se almacena el registro DNS), de modo que se actualice a través de Internet. Asegúrese de que guardó los cambios para que Microsoft pueda ver y comprobar el registro.
