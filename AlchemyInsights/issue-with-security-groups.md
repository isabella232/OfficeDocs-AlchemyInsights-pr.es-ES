---
title: Problema con los grupos de seguridad
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925758"
---
# <a name="issue-with-security-groups"></a>Problema con los grupos de seguridad

**Si recibe el error de red AADDS104**

Las reglas de grupo de seguridad de red no válidas son la causa más común de errores de red en Azure Active Directory Domain Services (AD DS). El grupo de seguridad de red para la red virtual debe permitir el acceso a puertos y protocolos específicos. Si estos puertos están bloqueados, la plataforma de Azure no podrá supervisar ni actualizar el dominio administrado. La sincronización entre Azure AD y Azure AD DS también se ve afectada. Asegúrese de mantener abiertos los puertos predeterminados para evitar interrupciones en el servicio.

Para comprender y resolver alertas comunes de problemas de configuración de grupos de seguridad de red, consulte [Agregar y comprobar grupos de seguridad](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
