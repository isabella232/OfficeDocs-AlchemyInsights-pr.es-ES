---
title: Transferir la propiedad de facturación de Azure
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840636"
---
# <a name="transfer-azure-billing-ownership"></a>Transferir la propiedad de facturación de Azure

Inicie sesión en el [portal de Azure](https://portal.azure.com/) como administrador de la cuenta de facturación que tiene la suscripción que quiere transferir. Si no está seguro de si es el administrador, o si necesita determinar quién es, vea [Determinar el administrador de facturación de la cuenta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Buscar en **Administración de costos + facturación**.
- Seleccione **Suscripciones** en el panel izquierdo. Según el acceso, es posible que tenga que seleccionar un ámbito de facturación y, a continuación, las **Suscripciones** o las **Suscripciones de Azure**.
- Seleccione **Transferir propiedad de facturación** para la suscripción que desea transferir
- Escriba la dirección de correo electrónico de un usuario que sea administrador de facturación de la cuenta que será el nuevo propietario de la suscripción y, a continuación, seleccione **enviar solicitud de transferencia**
- El usuario recibe un correo electrónico con instrucciones para revisar su solicitud de transferencia. Para aprobar la solicitud de transferencia, el usuario debe seleccionar el vínculo en el mensaje de correo electrónico y siga las instrucciones.

**Nota** : si se transfiere la propiedad de facturación de su suscripción a una cuenta de usuario en otro espacio empresarial de Azure AD, todas las asignaciones del [control de acceso basado en roles (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para administrar los recursos de la suscripción se eliminan de forma permanente. Solo el nuevo propietario tendrá acceso para administrar los recursos de la suscripción. Para obtener más información, vea [Transferir la suscripción a un usuario en otro espacio empresarial de Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos recomendados**

- [Transferir la propiedad de facturación de una suscripción de Azure a otra cuenta](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Acerca de la transferencia de la propiedad de facturación para una suscripción de Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transferencia de Visual Studio, Microsoft Partner Network (MPN) y Pay a medida que se dirigen las suscripciones de desarrollo y pruebas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Preguntas más frecuentes sobre la transferencia de propiedad](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Solucionar problemas de transferencia de propiedad](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
