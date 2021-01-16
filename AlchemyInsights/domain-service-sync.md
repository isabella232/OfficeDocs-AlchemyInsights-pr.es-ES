---
title: Sincronización del servicio de dominio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876520"
---
# <a name="domain-service-synchronization"></a>Sincronización del servicio de dominio

Los objetos y credenciales de un dominio administrado de Azure Active Directory Domain Services (Azure AD DS) se pueden crear localmente en el dominio o sincronizarse desde un inquilino de Azure Active Directory (Azure AD). Cuando implementas Azure AD DS por primera vez, se configura e inicia una sincronización un solo vía automática para replicar los objetos de Azure AD. Esta sincronización une vía sigue en ejecución en segundo plano para mantener el dominio administrado de Azure AD DS actualizado con los cambios de Azure AD. No se produce ninguna sincronización de Azure AD DS de vuelta a Azure AD.

Para obtener más información sobre la sincronización del servicio de dominio de Azure Active Directory, consulte [Sincronización de servicios de dominio.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization) 
