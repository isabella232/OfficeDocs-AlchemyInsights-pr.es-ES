---
title: Las sugerencias de directivas de DLP no funcionan
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679602"
---
# <a name="dlp-policy-tip-issues"></a>Problemas de la sugerencia de directiva DLP

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**Sugerencias de directivas de DLP**

Cuando se usan **directivas de DLP**, se puede informar a los usuarios de una infracción de directiva con las sugerencias de **Directiva**. Los administradores pueden configurar las sugerencias de directiva para que se muestren mientras se prueba la Directiva DLP o cuando la Directiva está en el modo de cumplimiento completo.
  
Para configurar sugerencias de directiva en su Directiva DLP en el centro de seguridad y cumplimiento en el modo de cumplimiento completo, haga lo siguiente:
  
- Asegúrese de que las sugerencias de Directiva se hayan **habilitado** en la regla DLP siguiendo los pasos que se describen [aquí](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).

- Asegúrese de que el **contenido coincida con** lo que se **necesita** para desencadenar la regla que se describe en este [artículo.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- Las sugerencias de directivas se muestran en OWA y Outlook. Sin embargo, al usar **Outlook 2013 o versiones posteriores**, las sugerencias de directiva solo se muestran en ciertas condiciones. Estas condiciones se enumeran a continuación: [condiciones admitidas para Outlook 2013 o posterior para mostrar sugerencias de directiva](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)

Para obtener más información sobre las sugerencias de directivas de DLP, vea: [Show Policy Tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)
  