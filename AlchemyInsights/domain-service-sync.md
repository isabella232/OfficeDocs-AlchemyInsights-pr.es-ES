---
title: Sincronización de servicios de dominio
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
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057875"
---
# <a name="domain-service-synchronization"></a>Sincronización de servicios de dominio

Los objetos y las credenciales de un dominio administrado de Azure Active Directory Domain Services (Azure AD DS) se pueden crear localmente en el dominio o sincronizarse desde un inquilino de Azure Active Directory (Azure AD). Al implementar Azure AD DS por primera vez, se configura e inicia una sincronización uni-way automática para replicar los objetos de Azure AD. Esta sincronización uni-way continúa en segundo plano para mantener el dominio administrado de Azure AD DS actualizado con los cambios de Azure AD. No se produce ninguna sincronización de Azure AD DS de nuevo a Azure AD.

Para obtener más información sobre Azure Active Directory de servicio de dominio, vea [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
