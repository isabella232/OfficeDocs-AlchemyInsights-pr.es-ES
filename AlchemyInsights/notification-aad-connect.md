---
title: Notificación AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898041"
---
# <a name="notification-aad-connect"></a>Notificación AAD Connect

- Asegúrese de que está autorizado a realizar la operación. Los administradores globales tienen acceso de forma predeterminada. Además, puede usar el control de acceso [basado en roles para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar el permiso de registro al colaborador.
- Asegúrese de que los puntos de conexión necesarios están habilitados y no bloqueados debido al firewall. Para obtener más información, vea [requisitos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- El registro puede producir un error debido a que la capa de red somete a la inspección SSL a la comunicación saliente.
- Asegúrese de que ha comprobado la configuración de notificaciones de Azure AD Connect Health y revise la configuración. Para comprender cómo configurar las opciones de notificación de las notificaciones de Azure AD Connect Health, consulte esta [guía](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Para obtener más información sobre el informe de sincronización de AAD Connect Health y cómo descargarlo, vea Informe de sincronización [de nivel de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Para solucionar problemas de [alertas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) de mantenimiento de AAD Connect siga la guía de solución de problemas de las alertas de actualización de datos de AAD Connect Health y para las preguntas más frecuentes, vea [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
