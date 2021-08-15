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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999257"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>No se puede iniciar sesión en Azure debido a problemas del explorador (el explorador se cuelga, sigue girando, no se carga, etc.)

Es posible que se le haya afectado una interrupción. Compruebe si hay una interrupción continua: [Estado de estado de Azure .](https://status.azure.com/status/history/)

Cierre sesión de todas las sesiones activas de Azure. Inicie un modo de incógnito o en privado del explorador web.

También puedes intentar actualizar el explorador, usar otro explorador, eliminar cookies de caché si no funciona anteriormente.

Más información: [Solucionar problemas de inicio de sesión](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**No se puede acceder a las suscripciones**

En [Azure Portal,](https://portal.azure.com/)asegúrese de que el directorio de Azure correcto está seleccionado en la cuenta de la parte superior derecha.

En el [Centro de cuentas de Azure,](https://account.windowsazure.com/Subscriptions)asegúrese de que la cuenta usada es el administrador de la cuenta.

Más información: Solucionar [problemas sin suscripciones encontradas](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**No se puede acceder al historial de facturación**

El administrador de la cuenta debe asegurarse de que el usuario que obtiene acceso a la información de facturación se agrega en Azure Active Directory como usuario invitado: Agregar o eliminar [un nuevo usuario.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

A continuación, el usuario debe tener un rol de administrador global: [Asignar un rol a los usuarios](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Tras ello, se puede conceder al usuario acceso de facturación mediante directivas RBAC: [Conceder acceso a la facturación.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos recomendados**

-   [No puedo iniciar sesión para administrar mi suscripción a Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)