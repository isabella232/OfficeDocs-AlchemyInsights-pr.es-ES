---
title: Problema con AAD Connect Health
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453301"
---
# <a name="problem-with-aad-connect-health"></a>Problema con AAD Connect Health

- Asegúrese de que está autorizado a realizar la operación. Los administradores globales tienen acceso de forma predeterminada. Además, puede usar el control de acceso [basado en roles para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar el permiso de registro al colaborador.
- Asegúrese de que los puntos de conexión necesarios están habilitados y no bloqueados debido al firewall. Para obtener más información, vea [requisitos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- El registro puede producir un error debido a que la capa de red somete a la inspección SSL a la comunicación saliente.
- Asegúrese de que ha comprobado la configuración de notificaciones de Azure AD Connect Health. Revise la configuración. Esta [guía](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) puede ayudarle a comprender cómo configurar las opciones de notificación para las notificaciones de estado de Azure AD Connect.
- Para obtener más información sobre el informe de sincronización de AAD Connect Health y cómo descargarlo, vea Informe de sincronización [de nivel de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Para solucionar problemas de alertas de estado de AAD Connect, siga la guía de solución de problemas de las alertas de actualización de datos de [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) y para las preguntas más frecuentes, vea Common [AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
