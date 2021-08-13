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
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985234"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Uno de los certificados de servicio de federación local está expirando

Para resolver este problema, siga estos pasos:
  
- Instale el Microsoft Azure Active Directory de Windows PowerShell en el equipo (si el módulo aún no está instalado). Para ello, vaya [a Azure Active Directory PowerShell para Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga los pasos de la sección "Escenario 1: El certificado de firma de tokens de AD FS expiró" del error "Hubo un problema al acceder al sitio" de AD FS cuando un usuario federado inicia sesión en [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)o Intune .
    
- Siga los pasos descritos en [How to update or repair the settings of a federated domain in Microsoft 365, Azure o Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Para obtener más información acerca de la renovación de certificados de federación, vea [Renovación de certificados para O365 y Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

