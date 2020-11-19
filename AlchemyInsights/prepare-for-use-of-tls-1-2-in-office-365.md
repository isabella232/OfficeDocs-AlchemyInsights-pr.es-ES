---
title: Prepararse para el uso de TLS 1.2 en Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085921"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="e1d28-102">Prepararse para el uso de TLS 1.2 en Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e1d28-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="e1d28-103">A partir del 31 de octubre de 2018, Microsoft 365 seguirá realizando la transición a TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="e1d28-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="e1d28-104">A partir del 15 de octubre de 2020, O365 iniciará el desuso de TLS 1.0 y 1.1 en el servicio.</span><span class="sxs-lookup"><span data-stu-id="e1d28-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="e1d28-105">La implementación de este cambio se completará en las próximas semanas y meses, pero los clientes deben asumir que no funcionarán las llamadas TLS 1.0 ni 1.1 al interactuar con O365 a partir del 15 de octubre de 2020.</span><span class="sxs-lookup"><span data-stu-id="e1d28-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="e1d28-106">Como se comunicó anteriormente (MC126199 en diciembre de 2017, MC128929 en febrero de 2018, MC186827 en julio de 2019 y MC218794 en julio de 2020), estamos trasladando todos nuestros servicios en línea a Transport Layer Security (TLS) 1.2+ para ofrecer el mejor cifrado de su clase y para garantizar que nuestro servicio sea más seguro, de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="e1d28-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="e1d28-107">Los clientes aún pueden optar por tener TLS 1.0 o 1.1 en sus servidores y recursos, pero deben asumir que solo TLS 1.2 o superior funcionará al interactuar con los recursos de O365.</span><span class="sxs-lookup"><span data-stu-id="e1d28-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="e1d28-108">Para más información acerca de estos cambios, consulte [aquí](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) y [aquí](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e1d28-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  