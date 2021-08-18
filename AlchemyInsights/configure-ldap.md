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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090429"
---
# <a name="configure-ldap"></a>Configurar LDAP

Para configurar LDAP, haga lo siguiente:

1. Compruebe el estado de su dominio en [Azure Portal](https://aka.ms/aadds-health).
1. Asegúrese de que hay disponible una suscripción válida de Azure AD y de que los Servicios de dominio de Azure AD están habilitados.
1. El certificado necesario para habilitar LDAP seguro debe obtenerse de una entidad de certificación pública de confianza o ser un certificado autofirmado.
1. Asegúrese de que el certificado sigue las [directrices necesarias](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Certificado no válido**
1. Para renovar un certificado, siga los pasos para crear un nuevo certificado y volver a cargarlo: [Configurar LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Para resolver problemas conocidos con alertas LDAP seguras en Azure Active Directory Domain Services, consulte [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
