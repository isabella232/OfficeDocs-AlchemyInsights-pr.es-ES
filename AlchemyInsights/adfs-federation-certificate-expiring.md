---
title: Expiración del certificado de Federación de AD FS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821968"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="4c5bc-102">Expiración del certificado de Federación de AD FS</span><span class="sxs-lookup"><span data-stu-id="4c5bc-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="4c5bc-103">Para resolver este problema, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="4c5bc-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="4c5bc-104">Instale el módulo de Microsoft Azure Active Directory para Windows PowerShell en el equipo (si el módulo aún no está instalado).</span><span class="sxs-lookup"><span data-stu-id="4c5bc-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="4c5bc-105">Para ello, vaya a [Administrar Azure AD con Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="4c5bc-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="4c5bc-106">Siga los pasos de la sección "Escenario 1: El certificado de firma de tokens de AD FS expiró" del error "Hubo un problema al acceder al sitio" de AD FS cuando un usuario federado inicia sesión en [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)o Intune .</span><span class="sxs-lookup"><span data-stu-id="4c5bc-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="4c5bc-107">Siga los pasos de Actualizar o reparar la configuración de un dominio [federado en Microsoft, Azure o Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="4c5bc-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="4c5bc-108">Para obtener más información sobre cómo renovar certificados de federación, vea Renovar certificados de federación [para Microsoft 365 y Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="4c5bc-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
