---
title: Problema con un solo usuario
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428829"
---
# <a name="problem-with-single-user"></a>Problema con un solo usuario

- Es posible que el usuario no se haya aprovisionado porque el servicio aún no ha tenido la oportunidad de evaluarlo. Revise las instrucciones sobre cuánto tarda el aprovisionamiento, así como la barra de progreso de la página de configuración de aprovisionamiento. Si el estado estable especificado en la sección de detalles adicionales es anterior a la fecha en que se creó/actualizó o eliminó el usuario, significa que aún no hemos evaluado al usuario. En este escenario, lo mejor que se puede hacer es esperar a que finalice el servicio de aprovisionamiento.

  - Tenga en cuenta que nuestro servicio solo tiene en cuenta los cambios realizados en un usuario en el sistema de origen (HR en la nube). Debe haber un cambio válido en el sistema de origen para que Azure AD detecte el cambio y lo fluya a Active Directory.
- El servicio de aprovisionamiento evaluó al usuario y determinó que no debe aprovisionarse:
  - Si ha establecido un filtro de ámbito basado en atributos, asegúrese de que el usuario cumple los criterios especificados.
  - Si los usuarios ya existen en el sistema de destino y el estado del usuario en la coincidencia de origen y destino, no realizaremos ninguna acción adicional.
- El servicio de aprovisionamiento intentó aprovisionar al usuario y falló. Para estos escenarios, revise la pestaña solución de problemas y recomendaciones de los registros de aprovisionamiento:
  - Es posible que falte un atributo obligatorio en el usuario en Active Directory local o Azure AD. Por ejemplo, las reglas de generación userPrincipalName o sAMAccountName no están generando el valor correcto.
  - El atributo de coincidencia (normalmente employeeId) no se resuelve para un usuario único en Active Directory local o Azure AD. Por ejemplo, hay dos usuarios con el mismo employeeId en AD y el servicio devuelve un código de error que indica entradas de destino duplicadas para la misma entrada de origen.

Para revisar los registros de un solo usuario y grupos, vea [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
