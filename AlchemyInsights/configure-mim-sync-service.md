---
title: Configurar el servicio de sincronización MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430770"
---
# <a name="configure-mim-sync-service"></a>Configurar el servicio de sincronización MIM

El servicio de sincronización de Microsoft Identity Manager (MIM) es un componente de MIM. Es un servicio local centralizado que almacena e integra información para organizaciones que tienen varios directorios y bases de datos locales. Es posible que pueda resolver el problema con la sincronización de MIM si el problema se abordó en una actualización reciente de MIM o si es uno de los otros problemas mencionados en la sección siguiente.

**Pasos recomendados**

1. Asegúrese de que está utilizando una actualización reciente de la sincronización de MIM y compruebe las [notas de la versión de la sincronización de MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) para determinar si el problema se ha resuelto en una actualización.
2. Si el problema es con el conector LDAP genérico, el SQL genérico, el Lotus Domino o el de los servicios Web, asegúrese de que está usando una actualización reciente de los [conectores genéricos](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Si una ejecución de sincronización de MIM se detiene con un error, consulte la tabla de [códigos de error de ejecución](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) para determinar las posibles causas.
4. Si la ejecución se detiene con **extension-dll-exception**, entonces haga clic en esas palabras para abrir la ventana de **propiedades del objeto del espacio conector**, y haga clic en **Seguimiento de pila...** para ver más información sobre la causa subyacente, tal y como se describe en [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Si el componente del Servicio de notificación de cambio de contraseña (PCNS) muestra el **error 6025** en el registro de eventos durante la sincronización de la contraseña, compruebe la guía para la solución problemas del [informe del error 6025 de PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Si la sincronización completa con el Agente de administración de servicio de FIM es lenta, compruebe la configuración de **crecimiento automático** para TempDB, como se describe en la [Solución de problemas de sincronización completa lenta o colgante](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Si se encuentra un error de servidor detenido con creación fallida a través de servicios web usando el Agente de administración de servicio de FIM, consulte [Información de soporte: creación fallida mediante servicios web](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) para obtener una descripción general de las causas.

