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
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736895"
---
# <a name="transfer-azure-billing-ownership"></a>Transferir la propiedad de facturación de Azure

Inicie sesión en el [portal de Azure](https://portal.azure.com/) como administrador de la cuenta de facturación que tiene la suscripción que quiere transferir. Si no está seguro de si es el administrador, o si necesita determinar quién es, vea [Determinar el administrador de facturación de la cuenta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Buscar en _Administración de costos + facturación_.
1. Seleccione **Suscripciones** en el panel izquierdo. Según el acceso, es posible que tenga que seleccionar un ámbito de facturación y, a continuación, las **Suscripciones** o las **Suscripciones de Azure**.
1. Seleccione **Transferir propiedad de facturación** para la suscripción que desea transferir
1. Escriba la dirección de correo electrónico de un usuario que sea administrador de facturación de la cuenta y que será el nuevo propietario de la suscripción. A continuación, seleccione **Enviar solicitud de transferencia**
1. El usuario recibe un correo electrónico con instrucciones para revisar su solicitud de transferencia. Para aprobar la solicitud de transferencia, el usuario debe seleccionar el vínculo en el mensaje de correo electrónico y seguir las instrucciones.

Si se transfiere la propiedad de facturación de su suscripción a una cuenta de usuario en otro espacio empresarial de Azure AD, todas las asignaciones del [control de acceso basado en roles (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para administrar los recursos de la suscripción se eliminan de forma permanente. Solo el nuevo propietario tendrá acceso para administrar los recursos de la suscripción. Para obtener más información sobre cómo cambiar de directorio para su suscripción, vea [Transferir la suscripción a un usuario en otro espacio empresarial de Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Nota importante sobre el efecto de esto en las facturas**_: si ha transferido la propiedad de la factura de una suscripción de Azure, los cargos se prorratearán. Podrá obtener acceso a las facturas de la siguiente forma:  

1. Seleccione su suscripción en la  [Página de suscripciones](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) en Azure Portal como [un usuario con acceso a las facturas](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), luego seleccione  **Facturas**.
1. Haga clic en  **Descargar factura** para ver una copia de su factura en PDF. Si el mensaje dice  _No disponible_, consulte  [¿Por qué no veo una factura del último período de facturación?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. También puede ver el uso diario haciendo clic en el **período de facturación** para obtener un PDF de su factura y una copia del archivo detallado de uso diario (.CSV). Para obtener más información, consulte [Obtener datos de factura y uso](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos recomendados**

- [Transferir la propiedad de facturación de una suscripción de Azure a otra cuenta](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Acerca de la transferencia de la propiedad de facturación para una suscripción de Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transferencia de Visual Studio, Microsoft Partner Network (MPN) y Pay a medida que se dirigen las suscripciones de desarrollo y pruebas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Preguntas más frecuentes sobre la transferencia de propiedad](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Solucionar problemas de transferencia de propiedad](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
