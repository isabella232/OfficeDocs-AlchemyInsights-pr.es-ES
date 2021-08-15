---
title: Problema con el atributo y el filtro de alcance
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960204"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problema con el atributo y el filtro de alcance

**Problema con valores UPN en conflicto**

El aprovisionamiento de usuarios de Workday para AD muestra un mensaje de error **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. La operación falló porque el valor UPN proporcionado para la adición / modificación no es único en todo el bosque. Detalles del error: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

El valor **userPrincipalName** que el conector del Workday intenta asignar al crear la cuenta de usuario de AD ya existe en el dominio objetivo de AD. Esto implica que o bien (1) el usuario ya existe y la comprobación de ID coincidente falló para el usuario o que (2) la regla de generación de UPN generó un valor conflictivo.

Aquí se muestran los pasos de resolución sugeridos:

Si el usuario ya existe y la comprobación de ID coincidente no pudo vincular la cuenta de Workday a la cuenta de Active Directory, verifique si el atributo de ID coincidente (normalmente **employeeID**), tanto en Workday como en AD, tiene una coincidencia exacta. Si no tienen una coincidencia, es un problema de datos que debe solucionarse. Por ejemplo, si el EmployeeID en Workday es 001052 y en AD es 1052, el motor de aprovisionamiento no podrá vincular las dos cuentas e intentará crear un usuario que ya exista. En este caso, la solución consiste en cambiar el valor de **EmployeeID** en AD para incluir los ceros iniciales para que sea 001052.
Si la expresión generadora de UPN no genera un valor único, considere usar la función de reduplicado **SelectUniqueValue** para generar un valor único cada vez.

**El Workday para el aprovisionamiento de usuarios de AD no establece el valor de atributo de administrador para la cuenta de usuario de AD**

El trabajo del Workday para el aprovisionamiento de usuarios de AD no establece el valor de atributo de **administrador** para las cuentas de usuario de AD. Hay dos escenarios posibles cuando se observa este comportamiento:

1. El administrador en el Workday no se puede resolver en una cuenta de usuario de AD correspondiente porque el administrador no es de su ámbito.
2. En un escenario de **múltiples dominios de AD**, el administrador del Workday no está presente en el mismo dominio que el usuario.

Pruebe estos pasos para solucionar el problema:

1. Si ha definido filtros del ámbito, primero verifique si el administrador está en su ámbito y si cumple con la cláusula del ámbito. Si el administrador no satisface el filtro del ámbito, cámbielo para que el administrador también esté dentro del ámbito de la operación de aprovisionamiento.
2. Si tiene varios dominios de AD, el conector tiene una limitación conocida de incapacidad para resolver las referencias de administrador entre dominios.

Para obtener más información sobre cómo configurar Workday para el aprovisionamiento automatizado, vea [Tutorial: configurar Workday para el aprovisionamiento automático de usuarios](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













