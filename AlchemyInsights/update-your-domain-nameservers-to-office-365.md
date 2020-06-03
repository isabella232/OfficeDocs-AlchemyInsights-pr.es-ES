---
title: Actualizar los servidores de nombre de dominio para que señalen a Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510301"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="08ef1-102">Actualizar los servidores de nombre de dominio para que señalen a Microsoft</span><span class="sxs-lookup"><span data-stu-id="08ef1-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="08ef1-103">Nota: Los cambios de Nameserver a veces pueden tardar hasta 48 horas en propagarse.</span><span class="sxs-lookup"><span data-stu-id="08ef1-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="08ef1-104">Para configurar su dominio con Microsoft, los servidores de nombres en su registrador deben actualizarse.</span><span class="sxs-lookup"><span data-stu-id="08ef1-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="08ef1-105">Cree o edite los registros del servidor DNS en el registrador de dominios.</span><span class="sxs-lookup"><span data-stu-id="08ef1-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="08ef1-106">Vaya al sitio web del registrador de dominios y busque el área donde puede modificar los servidores DNS.</span><span class="sxs-lookup"><span data-stu-id="08ef1-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="08ef1-107">Cree edite dos registros de servidores DNS para que coincidan con estos valores:</span><span class="sxs-lookup"><span data-stu-id="08ef1-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="08ef1-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="08ef1-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="08ef1-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="08ef1-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="08ef1-110">Guarde los cambios.</span><span class="sxs-lookup"><span data-stu-id="08ef1-110">Save changes.</span></span>

<span data-ttu-id="08ef1-111">También puede encontrar instrucciones detalladas en este artículo: [cambiar los servidores de nombres para configurar Microsoft 365 con cualquier registrador de dominios](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="08ef1-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  