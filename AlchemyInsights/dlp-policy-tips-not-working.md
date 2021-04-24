---
title: Sugerencias de directivas dlp no funcionan
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
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958719"
---
# <a name="dlp-policy-tip-issues"></a>Problemas de sugerencias de directiva DLP

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

Para configurar las sugerencias de directiva en la directiva DLP en el Centro de seguridad & cumplimiento en modo de aplicación completa, haga lo siguiente:

- Asegúrese de que las sugerencias de **directiva se hayan habilitado** en la regla DLP. Para ver los pasos, vea [Enviar notificaciones por correo electrónico y mostrar sugerencias de directivas para directivas DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).

- Asegúrese de que el contenido coincide con lo necesario para desencadenar la regla descrita en [Definiciones de](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)entidad de tipo de información confidencial .

- Las sugerencias de directiva se muestran en OWA y Outlook. Sin embargo, al usar Outlook 2013 o versiones posteriores, las sugerencias de directiva solo se muestran en determinadas condiciones. Para obtener la lista de condiciones específicas, vea [Condiciones admitidas para Outlook 2013](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)o posterior para mostrar sugerencias de directiva .

Para obtener información sobre las sugerencias de directiva DLP, vea [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and Support Matrix for DLP Policy [Tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).