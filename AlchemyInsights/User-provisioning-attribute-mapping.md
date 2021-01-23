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
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935396"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="ee744-102">Asignación de atributos de aprovisionamiento del usuario</span><span class="sxs-lookup"><span data-stu-id="ee744-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="ee744-103">Para solucionar los problemas conocidos de asignación de atributos, consulte [Asignaciones de atributo](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="ee744-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="ee744-104">Microsoft Azure Active Directory (AD) proporciona compatibilidad para el aprovisionamiento de usuarios para aplicaciones SaaS de terceros como Salesforce, G Suite y otras.</span><span class="sxs-lookup"><span data-stu-id="ee744-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="ee744-105">Si habilita el aprovisionamiento de usuarios para una aplicación SaaS de terceros, Azure Portal controla sus valores de atributo a través de las asignaciones de atributos.</span><span class="sxs-lookup"><span data-stu-id="ee744-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="ee744-106">Para obtener información sobre cómo personalizar las asignaciones de atributos predeterminadas, vea [Personalizar asignaciones de atributos de aprovisionamiento de usuarios para aplicaciones SaaS en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="ee744-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="ee744-107">Para obtener más información sobre el aprovisionamiento de usuarios de aplicaciones SaaS, vea [¿Qué es el aprovisionamiento automatizado de usuarios para aplicaciones SaaS en Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ee744-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="ee744-108">Al personalizar las asignaciones de atributo para el aprovisionamiento de usuarios, es posible que el atributo que quiere asignar no aparezca en la Lista de atributos de origen.</span><span class="sxs-lookup"><span data-stu-id="ee744-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="ee744-109">En el artículo [Sincronizar un atributo desde su Active Directory local con Azure AD para aprovisionar a una aplicación](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) se muestra cómo agregar el atributo que falta mediante la sincronización desde su AD local a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee744-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
