---
title: Aprovisionamiento de usuarios
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971356"
---
# <a name="user-provisioning"></a>Aprovisionamiento de usuarios

- Use la [funcionalidad de aprovisionamiento](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) a petición para aprovisionar un usuario y obtener diagnósticos detallados sobre los pasos que se han realizado.
- Para solucionar los posibles problemas durante el aprovisionamiento de usuarios y grupos, consulte la guía de solución de problemas [No se está aprovisionando ningún usuario](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Si observa que los usuarios no se están aprovisionando, consulte los [Registros de aprovisionamiento (versión preliminar)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) en Azure Active Directory (AD). Buscar entradas de registro que pertenezcan a un usuario específico.
- Reinicie periódicamente el aprovisionamiento para capturar los usuarios que se perdieron en un ciclo de aprovisionamiento anterior.
- Es posible que el usuario o el grupo no se hayan aprovisionado porque nuestro servicio aún no ha tenido la oportunidad de evaluar al usuario. Revise las instrucciones sobre cuánto tarda el aprovisionamiento, así como la barra de progreso de la página de configuración de aprovisionamiento. Si el estado estable especificado en la sección de detalles adicionales es anterior a la fecha en que se creó/actualizó o eliminó el usuario, significa que aún no hemos evaluado al usuario. En este escenario, lo mejor que se puede hacer es esperar a que finalice el servicio de aprovisionamiento. Si se ha alcanzado el estado estable, se recomienda realizar un reinicio desde la interfaz de usuario en Azure Portal.
  - Tenga en cuenta que nuestro servicio solo tiene en cuenta los cambios realizados en un usuario o grupo en el sistema de origen (Azure Active Directory). Si un usuario o grupo se quita directamente en la aplicación (por ejemplo, ServiceNow), no somos conscientes de esos cambios y no lo revierte en función del estado del usuario en el sistema de origen. En este escenario, es mejor revertir el cambio directamente en la aplicación de destino.
- Nuestro servicio evaluó el usuario o grupo y determinó que no debe aprovisionarse:
  - Si ha establecido el ámbito en usuarios y grupos asignados, compruebe si el usuario o grupo está asignado a la aplicación.
  - Si el usuario o grupo está asignado a la aplicación, asegúrese de que no están asignados al rol de acceso predeterminado. Este rol no se puede usar para el aprovisionamiento.
  - Si ha establecido un filtro de ámbito basado en atributos, asegúrese de que el usuario cumple los criterios especificados.
  - Si los usuarios ya existen en el sistema de destino y el estado del usuario en la coincidencia de origen y destino, no realizaremos ninguna acción adicional.
- Nuestro servicio intentó aprovisionar al usuario y falló. Para estos escenarios, revise la pestaña solución de problemas y recomendaciones de los registros de aprovisionamiento:
  - Es posible que falte un atributo obligatorio en el usuario Azure Active Directory o que no coincida con el formato requerido por la aplicación de terceros. Por ejemplo, el atributo Country de un usuario puede establecerse en Estados Unidos cuando debería ser ESTADOS UNIDOS.
  - El atributo es un atributo referencial que aún no existe en la aplicación de destino. Un atributo referencial es un atributo que apunta a otro objeto, por ejemplo, un usuario que es miembro de un grupo. El identificador del usuario estaría en el atributo member del grupo, pero solo se puede procesar si el objeto de usuario al que apunta ya existe.
