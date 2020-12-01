---
title: Eliminar espacio empresarial
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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477704"
---
# <a name="delete-tenant"></a>Eliminar espacio empresarial

Para eliminar Azure AD, asegúrese de lo siguiente:
- Es un administrador global en el directorio.
- NO ha iniciado sesión con una cuenta que tiene el directorio predeterminado, por ejemplo, contoso.onmicrosoft.com, en la cuenta firmada, como admin@contoso.onmicrosoft.com.
- Quite todas las aplicaciones activas del directorio antes de la eliminación. Para quitar las aplicaciones activas, vaya a registros de aplicaciones y quite las aplicaciones existentes.
- No hay suscripciones activas para los servicios en línea de Microsoft, como Microsoft Azure, Office 365 o Azure AD Premium asociados en el directorio. Transferir sus suscripciones o acelerar la cancelación de suscripciones activas a través de la facturación y soporte de Azure. Obtenga más información sobre cómo cancelar las suscripciones de Office 365 y Azure. Para obtener instrucciones sobre cómo asociar o agregar una suscripción existente a un inquilino, vea [Associate or Add a Azure Inscription to your Azure ad tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- No hay ninguna licencia activa. Para quitar licencias, consulte [How to Remove subscription to Remove License](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- No hay otros usuarios activos en el directorio, aparte del administrador global, al intentar eliminar Azure AD. Quite los demás usuarios activos y se deberán quitar todas las dependencias de un nombre de dominio personalizado en el inquilino, como los usuarios creados con admin@contoso.com.

Para obtener más información acerca de los pasos para:
- Eliminar "Azure Active Directory" o "suscripción", vea [eliminar Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Quitar aplicaciones del directorio, vea [quitar aplicaciones](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
