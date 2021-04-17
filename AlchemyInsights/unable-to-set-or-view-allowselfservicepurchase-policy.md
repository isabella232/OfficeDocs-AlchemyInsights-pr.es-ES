---
title: No se puede establecer ni ver la directiva AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826108"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="2955a-102">No se puede establecer ni ver la directiva AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="2955a-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="2955a-103">Al intentar establecer o ver la directiva AllowSelfServicePurchase, recibe el siguiente mensaje de error:</span><span class="sxs-lookup"><span data-stu-id="2955a-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="2955a-104">*HandleError: no se pudo recuperar la directiva de producto con PolicyId 'AllowSelfServicePurchase', ErrorMessage: se cerró la conexión subyacente: se produjo un error inesperado en un envío.*</span><span class="sxs-lookup"><span data-stu-id="2955a-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="2955a-105">Esto puede deberse a una versión anterior de Seguridad de la capa de transporte (TLS).</span><span class="sxs-lookup"><span data-stu-id="2955a-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="2955a-106">Para conectar el servicio MSCommerce, debe usar TLS 1.2 o posterior.</span><span class="sxs-lookup"><span data-stu-id="2955a-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="2955a-107">Pruebe los pasos siguientes para habilitar o establecer el protocolo TLS en 1.2, comprobar y reintentar.</span><span class="sxs-lookup"><span data-stu-id="2955a-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="2955a-108">En el símbolo del sistema de PowerShell (PS C: escriba el siguiente comando para establecer el protocolo \) TLS en la versión 1.2:</span><span class="sxs-lookup"><span data-stu-id="2955a-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="2955a-109">Compruebe los protocolos TLS en uso con el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="2955a-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="2955a-110">Reintente los comandos Get o Update según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="2955a-110">Retry the Get or Update commands as needed.</span></span>

