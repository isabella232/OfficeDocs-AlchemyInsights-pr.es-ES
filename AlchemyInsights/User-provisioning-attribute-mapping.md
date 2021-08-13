---
title: Asignación de atributos de aprovisionamiento del usuario
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918160"
---
# <a name="user-provisioning-attribute-mapping"></a>Asignación de atributos de aprovisionamiento del usuario

1. Para solucionar los problemas conocidos de asignación de atributos, consulte [Asignaciones de atributo](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) proporciona compatibilidad para el aprovisionamiento de usuarios para aplicaciones SaaS de terceros como Salesforce, G Suite y otras. Si habilita el aprovisionamiento de usuarios para una aplicación SaaS de terceros, Azure Portal controla sus valores de atributo a través de las asignaciones de atributos. Para obtener información sobre cómo personalizar las asignaciones de atributos predeterminadas, vea [Personalizar asignaciones de atributos de aprovisionamiento de usuarios para aplicaciones SaaS en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Para obtener más información sobre el aprovisionamiento de usuarios de aplicaciones SaaS, vea [¿Qué es el aprovisionamiento automatizado de usuarios para aplicaciones SaaS en Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Al personalizar las asignaciones de atributo para el aprovisionamiento de usuarios, es posible que el atributo que quiere asignar no aparezca en la Lista de atributos de origen. En el artículo [Sincronizar un atributo desde su Active Directory local con Azure AD para aprovisionar a una aplicación](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) se muestra cómo agregar el atributo que falta mediante la sincronización desde su AD local a Azure AD.
