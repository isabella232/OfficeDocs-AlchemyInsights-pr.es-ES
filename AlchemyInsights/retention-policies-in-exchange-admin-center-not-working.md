---
title: Directivas de retención en el Centro de administración de Exchange que no funcionan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952245"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Directivas de retención en el Centro de administración de Exchange

Si desea que ejecutemos comprobaciones automatizadas para la configuración mencionada a continuación, seleccione el botón atrás <-- en la parte superior de esta página y, a continuación, escriba la dirección de correo electrónico del usuario que tiene problemas con las directivas de retención.

Si tiene problemas con las directivas de retención en el Centro de administración de Exchange que no se aplican a buzones o elementos que no se mueven al buzón de archivo, compruebe lo siguiente:

**Causas raíz:**

- **El Asistente para carpetas** administradas no ha procesado el buzón del usuario. El Asistente para carpetas administradas intenta procesar todos los buzones de la organización basada en la nube una vez cada siete días.

  **Solución:** Ejecute el Asistente para carpeta administrada.

- **RetentionHold** se ha **habilitado** en el buzón. Si el buzón se ha colocado en retentionHold, la directiva de retención en el buzón no se procesará durante ese tiempo.

  **Solución:** Compruebe el estado de la configuración de retención y actualice según sea necesario. Para obtener más información, vea [Retención de buzones de correo.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Nota:** Si un buzón es menor que 10 MB, el Asistente para carpetas administradas no procesará automáticamente el buzón.
 
Para obtener más información sobre las directivas de retención en el Centro de administración de Exchange, vea:

- [Etiquetas de retención y directivas de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Aplicar una directiva de retención a buzones o](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Agregar o quitar etiquetas de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Cómo identificar el tipo de retención en un buzón](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
