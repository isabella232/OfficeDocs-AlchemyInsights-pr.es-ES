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
# <a name="configure-ldap"></a>Configurar LDAP

Para configurar LDAP, haga lo siguiente:

1. Compruebe el estado de su dominio en [Azure Portal.](https://aka.ms/aadds-health)
1. Asegúrese de que haya disponible una suscripción válida de Azure AD y de que se hayan habilitado los Servicios de dominio de Azure AD.
1. El certificado necesario para habilitar LDAP seguro debe obtenerse de una entidad de certificación pública de confianza o ser un certificado autofirmado.
1. Asegúrese de que el certificado sigue las instrucciones [necesarias.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Certificado no válido**
1. Para renovar un certificado, siga los pasos para crear un nuevo certificado y volver a cargarlo: [Configurar LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Para resolver el problema conocido con alertas LDAP seguras en Azure Active Directory Domain Services, consulte [Resolver alertas LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
