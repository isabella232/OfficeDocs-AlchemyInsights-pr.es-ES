---
title: Varios usuarios no ven los complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729888"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="a10a8-102">Varios usuarios no ven los complementos en Outlook</span><span class="sxs-lookup"><span data-stu-id="a10a8-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="a10a8-103">Si prueba los complementos de Outlook y no aparecen ninguno, como un primer paso de solución de problemas, use el cmdlet de PowerShell **Get-OrganizationConfig** para consultar el parámetro _AppsForOfficeEnabled_.</span><span class="sxs-lookup"><span data-stu-id="a10a8-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="a10a8-104">Si la consulta devuelve un valor de **False**, establezca este parámetro en **True** con el cmdlet **Set-OrganizationConfig**, para que los complementos se muestren de la forma esperada.</span><span class="sxs-lookup"><span data-stu-id="a10a8-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="a10a8-105">No se recomienda establecer el parámetro _AppsForOfficeEnabled_ en **False**.</span><span class="sxs-lookup"><span data-stu-id="a10a8-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="a10a8-106">Un valor **False** reemplaza todas las opciones de configuración de rol administrativo y de usuario anteriores y evita que todos los usuarios de la organización puedan activar aplicaciones nuevas.</span><span class="sxs-lookup"><span data-stu-id="a10a8-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="a10a8-107">Para obtener más información, consulte [Especifique los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="a10a8-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>