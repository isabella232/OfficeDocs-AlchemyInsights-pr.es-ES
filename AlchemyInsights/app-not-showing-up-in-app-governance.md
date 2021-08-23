---
title: Mi aplicación no aparece en Gobierno de aplicaciones
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362420"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Mi aplicación no aparece en Gobierno de aplicaciones

Si la aplicación no se muestra en App Governance, compruebe lo siguiente:

1. Vaya a [Azure AD](https://aad.portal.azure.com/) y busque el identificador de aplicación de la aplicación buscando el nombre de la aplicación en la barra superior de la página Información general.

1. Accede Graph Explorer y busca el identificador de aplicación en la entidad de servicio mediante esta consulta y reemplazando por el identificador de aplicación <appId> relevante: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Si no se devuelve ningún resultado, busque el identificador de aplicación dentro de la aplicación usando esta consulta y reemplazando por el identificador de aplicación <appId> relevante: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Si tiene problemas con la consulta, vea [Obtener soporte técnico](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Para obtener más información o información sobre tus aplicaciones en El gobierno de aplicaciones, consulta [Información sobre visibilidad e información.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Para obtener más información sobre cómo ver tus aplicaciones, [consulta Ver tus aplicaciones.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
