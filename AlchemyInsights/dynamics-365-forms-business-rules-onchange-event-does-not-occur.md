---
title: 'Reglas empresariales de Dynamics 365 Forms: regla de negocio que no se dispara para un formulario'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947316"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>El evento OnChange no se produce si el campo se cambia mediante programación

El *evento OnChange* no se produce si el campo se cambia mediante programación mediante el *atributo.* [setValue (método).](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Si desea que los controladores de eventos del evento *OnChange* se ejecuten después de establecer el valor, debe usar el método [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) del atributo *formContext.data.entity* en el código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
