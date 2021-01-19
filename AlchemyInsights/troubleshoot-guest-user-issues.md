---
title: Solucionar problemas de usuarios invitados
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897750"
---
# <a name="troubleshoot-guest-user-issues"></a>Solucionar problemas de usuarios invitados

1. Para obtener instrucciones sobre cómo administrar el acceso de invitado a las aplicaciones, vea Administrar el acceso de invitado con [revisiones de acceso de Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Agregue usuarios invitados al directorio en [Azure Portal:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)en este inicio rápido, agregará un nuevo usuario invitado a su directorio de Azure AD a través de Azure Portal, enviará una invitación y verá el aspecto del proceso de canje de invitaciones del usuario invitado.
1. [Agregar un usuario invitado con PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)en este inicio rápido, usará el comando New-AzureADMSInvitation para agregar un usuario invitado a su inquilino de Azure.
1. Para obtener información sobre cómo asignar usuarios y grupos a aplicaciones empresariales en Azure Active Directory (Azure AD), ya sea desde Azure Portal o mediante PowerShell, vea Administrar la asignación de usuarios para una aplicación en [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. La colaboración B2B de Azure Active Directory (Azure AD) funciona con la mayoría de las aplicaciones que se integran con Azure AD. En este [artículo,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)se proporcionan instrucciones para configurar algunas aplicaciones SaaS populares para su uso con Azure AD B2B.
1. Como organización que usa las capacidades de colaboración B2B de Azure Active Directory (Azure AD) para invitar a usuarios invitados de organizaciones asociadas a Azure AD, ahora puede proporcionar a estos usuarios B2B acceso a aplicaciones locales. Estas aplicaciones locales pueden usar la autenticación basada en SAML o la autenticación integrada de Windows (IWA) con delegación limitada de Kerberos (EAPD). Para obtener más información, vea [Conceder a los usuarios B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)de Azure AD acceso a las aplicaciones locales.
1. Obtenga información sobre cómo conceder a las cuentas de asociado administradas localmente acceso a recursos en la nube [mediante la colaboración B2B de Azure AD.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)