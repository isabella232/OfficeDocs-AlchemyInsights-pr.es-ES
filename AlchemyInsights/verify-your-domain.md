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
ms.openlocfilehash: 9e258cfc70c57fe787830d659dc52f4696768bea164d3be9ce7bcb9e7123c5a9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971032"
---
# <a name="verify-your-domain"></a>Verify your domain

 **Es probable que el registro no se haya actualizado en Internet.**
  
Normalmente, solo nos lleva unos minutos poder ver el nuevo registro, pero de vez en cuando puede tardar unas horas. 
  
- Si ya ha esperado tanto tiempo, compruebe que ha copiado y pegado el valor exacto en el registro de comprobación TXT en el host DNS. Uno de los problemas habituales es no incluir la parte de "MS=" del registro. ¡También la necesitamos!

- En algunos hosts DNS, tiene que llevar a cabo un paso adicional para guardar el archivo de zona (donde se almacena el registro DNS), de modo que se actualice a través de Internet. Asegúrese de que guardó los cambios para que Microsoft pueda ver y comprobar el registro.
