---
title: Acceso a la suscripción
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773782"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>No se puede iniciar sesión en Azure debido a problemas en el explorador (el explorador se bloquea, sigue girando, no se carga, etc.).

Es posible que se vea afectado por una interrupción. Compruebe si hay una interrupción continua: [Estado de Azure Health](https://status.azure.com/status/history/).

Cierre sesión en todas las sesiones de Azure activas. Inicie un modo en privado o incógnito de su explorador Web.

También puede intentar actualizar el explorador, usar otro explorador y eliminar las cookies de caché si no funciona.

Más información: [solución de problemas de inicio de sesión](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**No se puede tener acceso a las suscripciones**

En [Azure portal](https://portal.azure.com/), asegúrese de que se selecciona el directorio de Azure correcto en la cuenta de la parte superior derecha.

En el [centro de cuentas de Azure](https://account.windowsazure.com/Subscriptions), asegúrese de que la cuenta usada sea el administrador de la cuenta.

Más información: [solucionar problemas no se encontraron suscripciones](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**No se puede obtener acceso al historial de facturación**

El administrador de la cuenta debe asegurarse de que el usuario que tiene acceso a la información de facturación se agrega a Azure Active Directory como usuario invitado: [Agregar o eliminar un nuevo usuario](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

A continuación, el usuario debe tener un rol de administrador global: [asignar rol a los usuarios](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Registrar esto, al usuario se le puede conceder acceso a la facturación mediante directivas RBAC: [conceder acceso a la facturación](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos recomendados**

-   [No puedo iniciar sesión para administrar mi suscripción a Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)