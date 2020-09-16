---
title: Verify your domain
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
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734323"
---
# <a name="verify-your-domain"></a><span data-ttu-id="c2492-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="c2492-102">Verify your domain</span></span>

 <span data-ttu-id="c2492-103">**Es probable que el registro no se haya actualizado a través de Internet.**</span><span class="sxs-lookup"><span data-stu-id="c2492-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="c2492-104">Normalmente, solo se tarda unos minutos para poder ver el nuevo registro, pero en ocasiones puede tardar varias horas en realizarse.</span><span class="sxs-lookup"><span data-stu-id="c2492-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="c2492-105">Si ya ha esperado ese tiempo, compruebe que ha copiado y pegado el valor exacto en el registro de verificación TXT en el host DNS.</span><span class="sxs-lookup"><span data-stu-id="c2492-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="c2492-106">Uno de los problemas habituales es no incluir la parte de "MS=" del registro.</span><span class="sxs-lookup"><span data-stu-id="c2492-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="c2492-107">¡También la necesitamos!</span><span class="sxs-lookup"><span data-stu-id="c2492-107">We need that too!</span></span>

- <span data-ttu-id="c2492-108">En algunos hosts DNS, tiene que llevar a cabo un paso adicional para guardar el archivo de zona (donde se almacena el registro DNS), de modo que se actualice a través de Internet.</span><span class="sxs-lookup"><span data-stu-id="c2492-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="c2492-109">Asegúrese de que ha guardado los cambios para que Microsoft pueda ver y comprobar el registro.</span><span class="sxs-lookup"><span data-stu-id="c2492-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
