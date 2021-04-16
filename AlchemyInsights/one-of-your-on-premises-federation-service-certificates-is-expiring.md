---
title: Uno de los certificados de servicio de federación local está expirando
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810069"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="52402-102">Uno de los certificados de servicio de federación local está expirando</span><span class="sxs-lookup"><span data-stu-id="52402-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="52402-103">Para resolver este problema, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="52402-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="52402-104">Instale el módulo de Microsoft Azure Active Directory para Windows PowerShell en el equipo (si el módulo aún no está instalado).</span><span class="sxs-lookup"><span data-stu-id="52402-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="52402-105">Para ello, vaya a [Azure Active Directory PowerShell para Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="52402-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="52402-106">Siga los pasos de la sección "Escenario 1: El certificado de firma de tokens de AD FS expiró" del error "Hubo un problema al acceder al sitio" de AD FS cuando un usuario federado inicia sesión en [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)o Intune .</span><span class="sxs-lookup"><span data-stu-id="52402-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="52402-107">Siga los pasos de Cómo actualizar o reparar la configuración de un dominio federado en [Microsoft 365, Azure o Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="52402-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="52402-108">Para obtener más información acerca de la renovación de certificados de federación, vea [Renovación de certificados para O365 y Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="52402-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

