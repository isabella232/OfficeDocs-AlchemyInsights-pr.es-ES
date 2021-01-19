---
title: Problemas de consentimiento del administrador
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888323"
---
# <a name="admin-consent-issues"></a>Problemas de consentimiento del administrador

1. Habilite el flujo [de trabajo de consentimiento de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) administrador para permitir a los usuarios solicitar la aprobación del administrador directamente desde la pantalla de consentimiento.

1. Si usted o los usuarios de su aplicación están viendo errores inesperados durante el proceso de consentimiento, vea este artículo para conocer los pasos de solución de problemas: Error inesperado al dar su consentimiento [a una aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Obtenga más información sobre el consentimiento del [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) administrador en la plataforma de identidad de [Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)cómo funciona la solicitud de consentimiento y cómo evaluar una solicitud de consentimiento de administrador para todo [el espacio empresarial.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Las aplicaciones que se integran con la plataforma de identidad de Microsoft siguen un modelo de autorización que proporciona a los usuarios y administradores el control sobre cómo se puede acceder a los datos. La implementación del modelo de autorización se ha actualizado en el punto de conexión de la plataforma de identidad de Microsoft y cambia la forma en que una aplicación debe interactuar con la plataforma de identidad de Microsoft. Consulte [Permisos y consentimiento en el](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) punto de conexión de la plataforma de identidad de Microsoft para obtener información general sobre este modelo de autorización, incluidos los ámbitos, los permisos y el consentimiento.