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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952986"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiración del certificado de Federación de AD FS

Para resolver este problema, siga estos pasos:
  
1. Instale el Microsoft Azure Active Directory de Windows PowerShell en el equipo (si el módulo aún no está instalado). Para ello, vaya a [Administrar Azure AD con Windows PowerShell](https://aka.ms/aadposh).

2. Siga los pasos de la sección "Escenario 1: El certificado de firma de tokens de AD FS expiró" del error "Hubo un problema al acceder al sitio" de AD FS cuando un usuario federado inicia sesión en [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)o Intune .

3. Siga los pasos de Actualizar o reparar la configuración de un dominio [federado en Microsoft, Azure o Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para obtener más información acerca de la renovación de certificados de federación, vea [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
