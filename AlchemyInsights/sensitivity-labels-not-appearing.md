---
title: No aparecen las etiquetas de confidencialidad
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
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801201"
---
# <a name="sensitivity-labels-not-appearing"></a>No aparecen las etiquetas de confidencialidad

Las etiquetas de confidencialidad le permiten clasificar y ayudar a proteger el contenido confidencial. Se pueden crear en el centro de cumplimiento de Microsoft 365, el centro de seguridad de Microsoft 365 o el centro de cumplimiento de & de seguridad de Microsoft 365 en las etiquetas de confidencialidad > clasificación. Para obtener más información acerca de esta característica, consulte [información general sobre las etiquetas de confidencialidad](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Si ha configurado las etiquetas de confidencialidad pero no aparecen en las aplicaciones de Microsoft 365, compruebe lo siguiente:

- Confirme que la etiqueta de confidencialidad se ha [publicado](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) en los usuarios y grupos que desee.

- Confirme que el usuario usa una aplicación que admite etiquetas de confidencialidad (consulte [las etiquetas de confidencialidad en el documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)).

- Si va a [migrar las etiquetas de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), tenga en cuenta las consideraciones que se enumeran [aquí](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Compatibilidad con prevención de pérdida de datos (DLP): Actualmente, solo se pueden usar las etiquetas de retención como condición en las directivas de DLP.  La compatibilidad con las etiquetas de confidencialidad en una directiva DLP todavía no está disponible, pero estamos trabajando en ella.

- Si el cifrado está habilitado en una etiqueta de confidencialidad, puede elegir entre:
    - Asignar permisos ahora
    - Permitir a los usuarios asignar permisos


Para obtener más información sobre posibles problemas, consulte [problemas conocidos con las etiquetas de confidencialidad](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).