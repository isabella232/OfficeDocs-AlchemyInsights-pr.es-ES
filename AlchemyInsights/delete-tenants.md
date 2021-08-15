---
title: Eliminar inquilino
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993910"
---
# <a name="delete-tenant"></a>Eliminar inquilino

Para eliminar un Azure AD, asegúrese de:
- Es un administrador global en el directorio.
- NO ha iniciado sesión con una cuenta que tenga el directorio predeterminado, como contoso.onmicrosoft.com en la cuenta que ha iniciado sesión, como admin@contoso.onmicrosoft.com.
- Quite las aplicaciones activas del directorio antes de eliminar. Para quitar aplicaciones activas, vaya a Registros de aplicaciones y quite las aplicaciones existentes.
- No hay suscripciones activas para ninguna Microsoft Online Services, como Microsoft Azure, Office 365 o Azure AD Premium asociadas en el directorio. Transferir las suscripciones o acelerar la cancelación de suscripciones activas a través del soporte técnico y facturación de Azure. Obtenga más información sobre cómo cancelar Office 365 y suscripciones de Azure. Para obtener instrucciones sobre cómo asociar o agregar una suscripción existente a un inquilino, consulte Asociar o agregar una suscripción de Azure a su inquilino [de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- No hay ninguna licencia activa. Para quitar licencias, vea [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- No hay otros usuarios activos en el directorio además de usted como administrador global al intentar eliminar Azure AD. Quite cualquier otro usuario activo y las dependencias de un nombre de dominio personalizado en el inquilino también tendrán que quitarse, como los usuarios creados con admin@contoso.com.

Para obtener más información sobre cómo:
- Eliminar "Azure Active Directory" o "suscripción", vea [Eliminar Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Eliminación de aplicaciones en el directorio, vea [Quitar aplicaciones](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
