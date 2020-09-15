---
title: Conflictos con SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713471"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="ad353-102">Conflictos con SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad353-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="ad353-103">Si recibe errores durante la sincronización, como "Existe un objeto sincronizado con los mismos ProxyAddress o UserPrincipalName en el directorio", consulte [Diagnosticar y corregir los errores de sincronización de atributos duplicados](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="ad353-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="ad353-104">Asimismo, plantéese habilitar la resistencia de atributos duplicados.</span><span class="sxs-lookup"><span data-stu-id="ad353-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="ad353-105">Para más información, lea [Resistencia de atributo duplicado y sincronización de identidad](https://aka.ms/duplicateattributeresiliency)</span><span class="sxs-lookup"><span data-stu-id="ad353-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>