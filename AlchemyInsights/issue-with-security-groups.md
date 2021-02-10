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
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162947"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="1e597-102">Problema con los grupos de seguridad</span><span class="sxs-lookup"><span data-stu-id="1e597-102">Issue with security groups</span></span>

<span data-ttu-id="1e597-103">**Si recibe el error de red AADDS104**</span><span class="sxs-lookup"><span data-stu-id="1e597-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="1e597-104">Las reglas de grupo de seguridad de red no válidas son la causa más común de errores de red en Azure Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="1e597-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="1e597-105">El grupo de seguridad de red para la red virtual debe permitir el acceso a puertos y protocolos específicos.</span><span class="sxs-lookup"><span data-stu-id="1e597-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="1e597-106">Si estos puertos están bloqueados, la plataforma de Azure no podrá supervisar ni actualizar el dominio administrado.</span><span class="sxs-lookup"><span data-stu-id="1e597-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="1e597-107">La sincronización entre Azure AD y Azure AD DS también se ve afectada.</span><span class="sxs-lookup"><span data-stu-id="1e597-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="1e597-108">Asegúrese de mantener abiertos los puertos predeterminados para evitar interrupciones en el servicio.</span><span class="sxs-lookup"><span data-stu-id="1e597-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="1e597-109">Para comprender y resolver alertas comunes de problemas de configuración de grupos de seguridad de red, consulte [Agregar y comprobar grupos de seguridad](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="1e597-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
