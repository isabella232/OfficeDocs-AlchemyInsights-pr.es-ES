---
title: Problema con AAD Conectar Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923769"
---
# <a name="problem-with-aad-connect-health"></a>Problema con AAD Conectar Health

- Asegúrese de que está autorizado a realizar la operación. Los administradores globales tienen acceso de forma predeterminada. Además, puede usar el control de acceso [basado en roles para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar el permiso de registro al colaborador.
- Asegúrese de que los puntos de conexión necesarios están habilitados y no bloqueados debido al firewall. Para obtener más información, vea [requisitos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- El registro puede producir un error debido a que la capa de red somete a la inspección SSL a la comunicación saliente.
- Asegúrese de que ha comprobado la configuración de notificaciones de Azure AD Conectar Health. Revise la configuración. Esta [guía](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) puede ayudarle a comprender cómo configurar las opciones de notificación de Azure AD Conectar notificaciones de estado.
- Para obtener más información sobre el informe de sincronización Conectar estado de AAD y cómo descargarlo, vea Informe de sincronización [de nivel de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Para solucionar problemas de las alertas de mantenimiento de AAD Conectar, siga la guía de solución de problemas de las alertas de actualización de datos de [AAD Conectar Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) y para las preguntas más frecuentes, consulte Common [AAD Conectar Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
