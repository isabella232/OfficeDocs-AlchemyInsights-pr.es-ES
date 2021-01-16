---
title: Configurar LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876593"
---
# <a name="configure-ldap"></a><span data-ttu-id="b2030-102">Configurar LDAP</span><span class="sxs-lookup"><span data-stu-id="b2030-102">Configure LDAP</span></span>

<span data-ttu-id="b2030-103">Para configurar LDAP, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="b2030-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="b2030-104">Compruebe el estado de su dominio en [Azure Portal.](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="b2030-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="b2030-105">Asegúrese de que haya disponible una suscripción válida de Azure AD y de que se hayan habilitado los Servicios de dominio de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b2030-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="b2030-106">El certificado necesario para habilitar LDAP seguro debe obtenerse de una entidad de certificación pública de confianza o ser un certificado autofirmado.</span><span class="sxs-lookup"><span data-stu-id="b2030-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="b2030-107">Asegúrese de que el certificado sigue las instrucciones [necesarias.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)</span><span class="sxs-lookup"><span data-stu-id="b2030-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="b2030-108">**Certificado no válido**</span><span class="sxs-lookup"><span data-stu-id="b2030-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="b2030-109">Para renovar un certificado, siga los pasos para crear un nuevo certificado y volver a cargarlo: [Configurar LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b2030-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="b2030-110">Para resolver el problema conocido con alertas LDAP seguras en Azure Active Directory Domain Services, consulte [Resolver alertas LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b2030-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
