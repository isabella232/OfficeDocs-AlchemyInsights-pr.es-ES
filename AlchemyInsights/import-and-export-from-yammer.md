---
title: Importación y exportación desde Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: 3ead2702c2fbd26b2e5596e26e9189c2f97baf93c93ec3cbd57f15c855b5128e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54001499"
---
# <a name="import-and-export-from-yammer"></a>Importación y exportación desde Yammer

**Importación**

Las opciones de importación de usuarios varían según si la red de Yammer está en [Modo nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) o no.

- **Modo no nativo**: se puede importar a usuarios a grupos mediante [Añadir desde la Libreta de direcciones](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limitado a 100 usuarios) dentro de la configuración de grupos, o bien a la red a través de [Actualización masiva](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) dentro de Administrador de red.
- **Modo nativo**: las operaciones de suscripción a grupos y a la red deben realizarse desde el [portal de Administración de Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), el [portal de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) o mediante otra opción de Azure AD. Las redes en Modo nativo ya no tienen acceso a la Actualización masiva y otras funciones heredadas.

> [!IMPORTANT]
> Yammer nunca fue compatible con la importación de contenido desde el Administrador de red, incluso cuando la característica de Exportación de datos se usó en otra red. Las soluciones de asociados o las API de REST de Yammer pueden volver a publicar el contenido.

**Exportación**

La [Exportación de datos de red dentro del Administrador de red](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permite exportar contenido de redes de Yammer, incluyendo mensajes y archivos. Los archivos adjuntos pueden ser extremadamente grandes y harán que las exportaciones tarden un tiempo considerable en completarse. Recomendamos que las redes activas se exporten utilizando la [API de exportación de datos](https://developer.yammer.com/docs/data-export-api) en partes por día o por semana. El soporte técnico de Microsoft no proporciona scripts personalizados para este propósito.

Existe una [exportación de RGPD](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) separada para exportar contenido para un usuario individual.