---
title: Solucionar problemas de usuario invitado
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939396"
---
# <a name="troubleshoot-guest-user-issues"></a>Solucionar problemas de usuario invitado

1. Para obtener instrucciones sobre cómo administrar el acceso de invitado a aplicaciones, consulte [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Agregar usuarios invitados al directorio en [Azure Portal:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)en esta guía de inicio rápido, agregará un nuevo usuario invitado al directorio de Azure AD a través de Azure Portal, enviará una invitación y verá cómo es el proceso de canje de invitaciones del usuario invitado.
1. Agregar un usuario invitado con [PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)en esta guía de inicio rápido, usará el comando New-AzureADMSInvitation para agregar un usuario invitado al inquilino de Azure.
1. Para obtener información sobre cómo asignar usuarios y grupos a aplicaciones empresariales en Azure Active Directory (Azure AD), ya sea desde Azure Portal o mediante PowerShell, consulte Manage [user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) La colaboración B2B funciona con la mayoría de las aplicaciones que se integran con Azure AD. En este [artículo,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)le explicamos las instrucciones para configurar algunas aplicaciones SaaS populares para su uso con Azure AD B2B.
1. Como organización que usa las capacidades de colaboración B2B de Azure Active Directory (Azure AD) para invitar a usuarios invitados de organizaciones asociadas a Azure AD, ahora puede proporcionar a estos usuarios B2B acceso a aplicaciones locales. Estas aplicaciones locales pueden usar la autenticación basada en SAML o la autenticación Windows integrada (IWA) con delegación limitada de Kerberos (KCD). Para obtener más información, vea [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Obtenga información sobre cómo conceder acceso a las cuentas de socio administradas localmente a recursos en la nube [mediante la colaboración B2B de Azure AD.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)