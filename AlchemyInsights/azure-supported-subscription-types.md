---
title: Tipos de suscripciones admitidas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791579"
---
# <a name="supported-subscription-types"></a>Tipos de suscripciones admitidas

Revise los tipos de suscripción admitidos para seguir adelante.

[Tipos de suscripciones admitidas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transferir la propiedad de la facturación**

Azure Portal como el [Administrador de la cuenta](https://ms.portal.azure.com/) de la facturación de la cuenta que tiene la suscripción que desea transferir

- Buscar en **Administración de costos + facturación** . Seleccione **suscripciones** en el panel izquierdo. Según el acceso, es posible que tenga que seleccionar un ámbito de facturación y, a continuación, las **suscripciones** o las **suscripciones de Azure** .
- Seleccione transferir propiedad de facturación para la suscripción que desea transferir
- Escriba la dirección de correo electrónico de un usuario que sea administrador de facturación de la cuenta que será el nuevo propietario de la suscripción y, a continuación, seleccione **enviar solicitud de transferencia**
- El usuario recibe un correo electrónico con instrucciones para revisar su solicitud de transferencia. Para aprobar la solicitud de transferencia, el usuario debe seleccionar el vínculo en el mensaje de correo electrónico y siga las instrucciones.

Nota: si se transfiere la propiedad de facturación de su suscripción a una cuenta de usuario en otro espacio empresarial de Azure AD, todas las asignaciones del [control de acceso basado en roles (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para administrar los recursos de la suscripción se eliminan de forma permanente. Solo el nuevo propietario tendrá acceso para administrar los recursos de la suscripción. Para obtener más información, vea [Transferir la suscripción a un usuario en otro espacio empresarial de Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Transferir la propiedad de la suscripción**

Requisitos previos basados en la función de transferencia de propiedad de la suscripción (RBAC) para administrar recursos en la suscripción pierde el acceso. Para obtener más información sobre cómo agregar una suscripción existente a un espacio empresarial, vea [Asociar o agregar una suscripción de Azure a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- La transferencia de la suscripción con una cantidad pendiente del ciclo de facturación actual no se transferirá al nuevo instrumento de pago de la nueva cuenta. La única información disponible para los usuarios en nueva cuenta es el costo del último mes de su suscripción. El resto del historial de uso y facturación no se transfiere con la suscripción.
- Transferir la propiedad de facturación de las suscripciones del contrato Enterprise (EA) actualmente solo se admite en el portal de contratos Enterprise
- La transferencia de una suscripción orientada a créditos como Visual Studio, BizSpark y Microsoft Partner Network a un nuevo usuario requiere una licencia de Visual Studio/Microsoft Partner Network para aceptar la solicitud de transferencia
- Todos los recursos como máquinas virtuales, discos y sitios web se transfieren a la nueva cuenta con éxito. Los siguientes recursos podrían verse afectados en una transferencia de suscripción entre espacios empresariales:

**Azure AD Domain Services**

Azure Key Vaults

- [Bases de datos y usuarios relacionados con SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), especialmente si el cliente usa una autenticación relacionada con Azure Active Directory.
- **Servicios de aplicaciones** configurados con la autenticación de Azure Active Directory podrían verse afectados
- Las cuentas de **Visual Studio Team** Services conectadas a las suscripciones de Azure pueden perder temporalmente el acceso cuando se cancela la suscripción de Azure conectada

**Documentos recomendados**

Pasos después de aceptar la propiedad de facturación:

- Para mantener la propiedad de la facturación, pero cambiar su tipo de suscripción, consulte: [Cambiar su suscripción de Azure a otra oferta](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transferencia de Visual Studio, Microsoft Partner Network (MPN) y Pay a medida que se dirigen las suscripciones de desarrollo y pruebas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transferir la propiedad de facturación de las suscripciones de contrato Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Preguntas más frecuentes sobre la transferencia de propiedad](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Solucionar problemas de transferencia de propiedad](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)