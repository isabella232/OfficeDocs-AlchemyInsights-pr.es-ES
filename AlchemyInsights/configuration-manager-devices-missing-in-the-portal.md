---
title: Faltan dispositivos de Configuration Manager en el portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812168"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="531db-102">Faltan dispositivos de Configuration Manager en el portal</span><span class="sxs-lookup"><span data-stu-id="531db-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="531db-103">Para que funcione la sincronización de dispositivos, debe poder accederse a los [puntos de conexión de Internet necesarios](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) desde el servidor local que hospeda el rol de punto de conexión de servicio.</span><span class="sxs-lookup"><span data-stu-id="531db-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="531db-104">Para solucionar problemas de sincronización de dispositivos, revise el archivo **CMGatewaySyncUploadWorker.log** que encontrará en el punto de conexión de servicio.</span><span class="sxs-lookup"><span data-stu-id="531db-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="531db-105">Obtenga más información sobre la [asociación de inquilinos en Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="531db-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
