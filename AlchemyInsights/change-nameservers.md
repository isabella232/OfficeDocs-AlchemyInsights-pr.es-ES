---
title: Cambiar NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714741"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="982b6-102">Actualizar los servidores de nombre de dominio para que señalen a Microsoft</span><span class="sxs-lookup"><span data-stu-id="982b6-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="982b6-103">Nota: Los cambios de Nameserver a veces pueden tardar hasta 48 horas en propagarse.</span><span class="sxs-lookup"><span data-stu-id="982b6-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="982b6-p101">Para configurar su dominio en Microsoft 365, los servidores DNS en su registrador deben actualizarse. Cree o edite los registros del servidor DNS en el registrador de dominios.</span><span class="sxs-lookup"><span data-stu-id="982b6-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="982b6-106">Vaya al sitio web del registrador de dominios y busque el área donde puede modificar los servidores DNS.</span><span class="sxs-lookup"><span data-stu-id="982b6-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="982b6-107">Cree edite dos registros de servidores DNS para que coincidan con estos valores:</span><span class="sxs-lookup"><span data-stu-id="982b6-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="982b6-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="982b6-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="982b6-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="982b6-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="982b6-110">Guarde los cambios.</span><span class="sxs-lookup"><span data-stu-id="982b6-110">Save changes.</span></span>

<span data-ttu-id="982b6-111">También encontrará instrucciones detalladas en este artículo: [Cambiar los servidores DNS con cualquier registrador de dominio](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="982b6-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  