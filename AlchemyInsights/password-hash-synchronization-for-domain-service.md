---
title: Sincronización de hash de contraseña para el servicio de dominio
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162940"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="1b17a-102">Sincronización de hash de contraseña para el servicio de dominio</span><span class="sxs-lookup"><span data-stu-id="1b17a-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="1b17a-103">**Si su instancia de Azure AD DS le pide que habilite la sincronización de hash de contraseña**</span><span class="sxs-lookup"><span data-stu-id="1b17a-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="1b17a-104">Se encuentra con un escenario en el que está ejecutando un entorno híbrido con usuarios que realizan sincronizaciones desde un entorno local de Azure Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="1b17a-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="1b17a-105">Esto se da a pesar de que tiene configurada la sincronización de hash de contraseña desde la instancia de AD DS local con su inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b17a-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="1b17a-106">**Causa**</span><span class="sxs-lookup"><span data-stu-id="1b17a-106">**Cause**</span></span>

<span data-ttu-id="1b17a-107">Esto sucede porque Azure AD Connect no sincroniza de forma predeterminada los hashes de Kerberos y New Technology LAN Manager (NTLM) heredados que son necesarios para Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="1b17a-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="1b17a-108">**Solución alternativa**</span><span class="sxs-lookup"><span data-stu-id="1b17a-108">**Workaround**</span></span> 

<span data-ttu-id="1b17a-109">Necesitará configurar Azure AD Connect para sincronizar los hashes de contraseña necesarios para la autenticación NTLM y Kerberos.</span><span class="sxs-lookup"><span data-stu-id="1b17a-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="1b17a-110">Después de configurar Azure AD Connect, un evento de cambio de contraseña o de creación de cuenta local también sincroniza los hashes de contraseña heredados con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b17a-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="1b17a-111">Haga clic [aquí](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) para obtener más información sobre esto, así como instrucciones sobre cómo habilitar la sincronización de contraseñas en entornos híbridos de Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="1b17a-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>