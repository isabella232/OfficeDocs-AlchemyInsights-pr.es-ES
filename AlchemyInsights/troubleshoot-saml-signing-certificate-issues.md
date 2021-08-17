---
title: Solución de problemas de firma de certificados de SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 290e740ccd7f3beac5b77e63c32c5b18c295070e6002dcdde44ce4a93f4330f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105693"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Solución de problemas de firma de certificados de SAML

Para resolver el problema del certificado de firma de SAML, siga los pasos recomendados:

1. Al agregar una aplicación empresarial que sea compatible con SSO, Azure generará un certificado denominado [Certificado de firma SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Este certificado tiene una fecha de expiración de 3 años. Para cambiar la fecha de expiración del certificado, vea [Personalizar la fecha de expiración del certificado de federación y extenderla a un nuevo certificado](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure usará este certificado para firmar los tokens SAML solicitados por la aplicación y enviarlos a la aplicación para un SSO correcto. Para que se complete, descargue el certificado desde Azure Portal y envíelo al proveedor de la aplicación para completar el proceso de SSO.

Cuando se complete este proceso, la aplicación confiará en este certificado y aceptará todos los tokens de SAML firmados con este certificado.

3. Si este certificado expira, cree uno nuevo, actualícelo en el proveedor de la aplicación y, después, actívelo en Azure. Para obtener más información, consulte [Renovar un certificado que pronto expirará](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Si el certificado expira, el usuario no se bloqueará.

4. [Agregue una dirección de correo electrónico para las notificaciones](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) que deba recibir antes de que expire el certificado actual.

> [!NOTE]
> El paso 4 es opcional.

5. Cambie las opciones de firma del certificado SAML de una aplicación y el algoritmo de firma de certificados. Para obtener más información, consulte [Cambiar las opciones de firma de certificado y la firma del algoritmo](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

