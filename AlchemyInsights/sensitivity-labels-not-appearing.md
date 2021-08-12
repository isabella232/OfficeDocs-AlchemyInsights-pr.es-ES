---
title: Etiquetas de confidencialidad que no aparecen
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061449"
---
# <a name="sensitivity-labels-not-appearing"></a>Etiquetas de confidencialidad que no aparecen

Las etiquetas de confidencialidad permiten clasificar y proteger el contenido confidencial. Se pueden crear en el centro de Centro de cumplimiento de Microsoft 365, Microsoft 365 seguridad o en Microsoft 365 de seguridad & cumplimiento en Clasificación > confidencialidad. Para obtener más información sobre esta característica, vea [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Si configuró las etiquetas de confidencialidad pero no aparecen en las aplicaciones Microsoft 365, compruebe lo siguiente:

- Confirme que la etiqueta de confidencialidad se [ha publicado](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) para los usuarios y grupos que desee.

- Confirme que el usuario usa una aplicación que admite etiquetas de confidencialidad: vea [etiquetas de confidencialidad en el documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Si va a migrar [etiquetas de Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)tenga en cuenta las consideraciones que se enumeran [aquí](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Compatibilidad con prevención de pérdida de datos (DLP): actualmente, solo se pueden usar etiquetas de retención como condición en las directivas DLP.  La compatibilidad con etiquetas de confidencialidad en una directiva DLP aún no está disponible, pero estamos trabajando en ella.

- Cuando el cifrado está habilitado en una etiqueta de confidencialidad, puede elegir entre:
    - Asignar permisos ahora
    - Permitir a los usuarios asignar permisos


Para obtener más información sobre posibles problemas, vea [Problemas conocidos con etiquetas de confidencialidad.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)