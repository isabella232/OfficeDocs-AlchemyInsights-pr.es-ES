---
title: Problema de aprovisionamiento de SCIM
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935407"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="401cc-102">Problema de aprovisionamiento de SCIM</span><span class="sxs-lookup"><span data-stu-id="401cc-102">SCIM provisioning issue</span></span>

<span data-ttu-id="401cc-103">El aprovisionamiento automático hace referencia a la creación de identidades de usuario y roles en las aplicaciones de la nube a los que los usuarios necesitan acceder.</span><span class="sxs-lookup"><span data-stu-id="401cc-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="401cc-104">Además de crear identidades de usuario, el aprovisionamiento automático incluye el mantenimiento y la eliminación de identidades de usuario como cambios de estado o roles.</span><span class="sxs-lookup"><span data-stu-id="401cc-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="401cc-105">Antes de iniciar la implementación, puede revisar [Cómo funciona el aprovisionamiento](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) para obtener la información que necesita saber sobre el aprovisionamiento de Azure Active Directory (AD) y obtener recomendaciones de configuración.</span><span class="sxs-lookup"><span data-stu-id="401cc-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="401cc-106">Como desarrollador de aplicaciones, puede usar la API de administración de usuarios del Sistema de administración de identidades entre dominios (SCIM) para habilitar el aprovisionamiento automático de los usuarios y grupos entre su aplicación y Azure AD.</span><span class="sxs-lookup"><span data-stu-id="401cc-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="401cc-107">En el artículo [Crear un punto de conexión y configurar el aprovisionamiento de usuarios con Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) se describe cómo compilar un punto de conexión SCIM e integrarlo con el servicio de aprovisionamiento de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="401cc-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



