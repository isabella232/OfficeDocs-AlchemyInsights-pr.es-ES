---
title: Configuración del servicio de aprovisionamiento
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480757"
---
# <a name="configuring-the-provision-service"></a>Configuración del servicio de aprovisionamiento

Para que el aprovisionamiento automatizado de usuarios funcione, Azure AD requiere credenciales válidas que le permitan conectarse a la API de Servicios web de Workday. Además, el botón Probar conexión de la aplicación aprovisionamiento de usuarios de Workday a AD también valida si puede conectarse al agente de aprovisionamiento de Azure AD Connect asociado al dominio de AD.

Si Azure Portal devuelve un error al guardar las credenciales, siga los pasos recomendados a continuación:

1. Confirme que ha configurado la cuenta de usuario de Workday Integration System tal como se indica en la sección tutorial Configurar usuario del sistema de [integración en Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Confirme que el servicio de agente de aprovisionamiento de Azure AD Connect está en funcionamiento en el servidor windows local mediante la Consola de administración de servicios. También puede comprobar el estado del agente en Azure Portal haciendo clic en el botón Ver agentes locales.
3. Asegúrese de escribir el valor del campo "Nombre de usuario de workday" con el formato username@workday-tenant-name. Si falta el nombre de workday-tenant, se produce un error en la autenticación de Workday.
4. Si va a configurar la integración con el inquilino de implementación de Workday, tenga en cuenta las horas de inactividad programadas del inquilino de Workday. Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.
5. En raras ocasiones, también puede ver este error si la contraseña del usuario del sistema de integración cambió debido a la actualización del inquilino o si la cuenta está en estado bloqueado o expirado. Compruebe el estado del usuario del sistema de integración con el administrador de Workday.

Para obtener más información sobre cómo configurar Workday para el aprovisionamiento automatizado, vea [Tutorial: configurar Workday para el aprovisionamiento automático de usuarios](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
