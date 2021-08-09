---
title: Flujo de trabajo no se está iniciando
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907755"
---
# <a name="workflow-is-not-starting"></a>Flujo de trabajo no se está iniciando

- SharePoint 2010 y SharePoint flujos de trabajo de 2013 no se inician.

    - Si el flujo de trabajo no se inicia, puede haber un problema de servicio temporal en el que los usuarios pueden experimentar retrasos intermitentes con el progreso del flujo de trabajo. Compruebe el [Panel de estado del servicio](https://admin.microsoft.com/AdminPortal/Home/servicehealth) para ver si su organización está afectada.

    - Si han pasado más de 24 horas desde que vio por primera vez este problema, registre un vale de soporte técnico. En muchos casos, ya estamos trabajando en una solución. Por favor, dénos al menos 24 horas para completar una solución.

- SharePoint flujos de trabajo de 2010 se retrasaron al inicio.

    - Esto ocurre si el flujo de trabajo se desencadena en lotes grandes. (por ejemplo, cuando se agregan varios elementos a la vez).

    - Los flujos de trabajo no están diseñados para ejecutarse en tiempo real, por lo que un retraso es un comportamiento por diseño.

   -  Si el flujo de trabajo es complejo Extensible Object Markup Language (XMOL), la compilación puede ser lenta. Consulte [este](https://support.microsoft.com//kb/3043697) artículo.

    - Debe simplificar el flujo de trabajo o rediseñar el flujo de trabajo con el tipo de plataforma de flujo de trabajo de Microsoft SharePoint 2013.

    - Si el historial de flujo de trabajo se ha hecho grande, es posible que desee purgar los elementos o crear una lista de historial nueva.

        Más información: [Purgar historial de flujos de trabajo](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Temas relacionados
¿Quieres probar Microsoft Flow en SharePoint Online?
- [Crear Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint y Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
