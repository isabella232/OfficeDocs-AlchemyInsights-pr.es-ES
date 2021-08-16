---
title: Notificación AAD Conectar
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
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097323"
---
# <a name="notification-aad-connect"></a>Notificación AAD Conectar

- Asegúrese de que está autorizado a realizar la operación. Los administradores globales tienen acceso de forma predeterminada. Además, puede usar el control de acceso [basado en roles para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar el permiso de registro al colaborador.
- Asegúrese de que los puntos de conexión necesarios están habilitados y no bloqueados debido al firewall. Para obtener más información, vea [requisitos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- El registro puede producir un error debido a que la capa de red somete a la inspección SSL a la comunicación saliente.
- Asegúrese de que ha comprobado la configuración de notificaciones de Azure AD Conectar Health y revise la configuración. Para comprender cómo configurar las opciones de notificación para notificaciones de Azure AD Conectar de mantenimiento, consulte esta [guía](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Para obtener más información sobre el informe de sincronización Conectar estado de AAD y cómo descargarlo, vea Informe de sincronización [de nivel de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Para solucionar problemas de AAD Conectar Health Alerts siga la guía de solución de problemas de las alertas de actualización de datos de mantenimiento de [AAD Conectar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) y para las preguntas más frecuentes, consulte [Common AAD Conectar Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
