---
title: Acerca de los administradores de Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995293"
---
# <a name="about-yammer-admins"></a>Acerca de los administradores de Yammer

**Administradores de red**

Los administradores globales se promueven automáticamente al rol De administrador verificado en una red de Yammer. En los siguientes casos, es posible que esta promoción no se produzca correctamente:

- Existen varias redes de Yammer y el administrador ha iniciado sesión en la incorrecta. [La consolidación](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) de red es necesaria para llegar a una red de Yammer.
- Se está utilizando Pim de Azure. Es posible que el usuario no sea promovido a administrador global lo suficiente como para que se produzca la promoción. Una actualización futura de Yammer puede resolver este problema, pero lo mejor es promover manualmente a los usuarios al administrador global.
- Existe un problema de sincronización con la red de Yammer. En este caso, se requiere una solicitud de soporte técnico para una investigación posterior.

Para obtener más información acerca de los roles de administrador de Yammer, vea [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Administradores de grupo**

Los administradores de grupos para grupos conectados de Microsoft 365 se sincronizan con la pertenencia a grupos de Azure AD. Para grupos grandes, esta sincronización puede tardar un período prolongado.
