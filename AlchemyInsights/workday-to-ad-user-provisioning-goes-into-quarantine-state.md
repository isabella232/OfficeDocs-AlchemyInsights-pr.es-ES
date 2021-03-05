---
title: El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430774"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena

**El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena y no se crean usuarios en AD**

El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena y los registros de auditoría muestran eventos de error de exportación con el mensaje **Error: OperationsError-SvcErr: Se produjo un error de operación. No se ha configurado ninguna referencia superior para el servicio de directorio. Por lo tanto, el servicio de directorio no puede emitir referencias a los objetos externos a este bosque**. Este error suele mostrarse si la unidad organizativa del contenedor de Active Directory no se ha configurado correctamente o si hay problemas con la asignación de expresiones usada para **parentDistinguishedName**.

Compruebe la unidad organizativa predeterminada para **Nuevos usuarios** de errores tipográficos. Asegúrese de que la unidad organizativa especificada ya existe en su AD. Si usa **parentDistinguishedName** en la asignación de atributos, asegúrese de que siempre se evalúa como un contenedor conocido dentro del dominio de AD. Compruebe el evento Exportar en los registros de auditoría para ver el valor generado.

Para obtener más información sobre cómo configurar Workday para el aprovisionamiento automatizado, vea [Tutorial: configurar Workday para el aprovisionamiento automático de usuarios](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

