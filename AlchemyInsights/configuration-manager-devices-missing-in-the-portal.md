---
title: Faltan dispositivos de Configuration Manager en el portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817261"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Faltan dispositivos de Configuration Manager en el portal

Para que funcione la sincronización de dispositivos, debe poder accederse a los [puntos de conexión de Internet necesarios](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) desde el servidor local que hospeda el rol de punto de conexión de servicio. Para solucionar problemas de sincronización de dispositivos, revise el archivo **CMGatewaySyncUploadWorker.log** que encontrará en el punto de conexión de servicio.

Obtenga más información sobre la [asociación de inquilinos en Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
