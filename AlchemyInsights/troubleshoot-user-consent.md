---
title: Solucionar problemas de consentimiento del usuario
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007915"
---
# <a name="troubleshoot-user-consent"></a>Solucionar problemas de consentimiento del usuario

1. Puede configurar cómo los usuarios finales consienten las aplicaciones a través de Azure Portal o PowerShell. Consulta [Configuración del consentimiento del usuario](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para obtener más información.
1. Un administrador también puede usar la [API de Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para conceder consentimiento a permisos delegados en nombre de un único usuario. Para obtener más información, vea [Obtener acceso en nombre de un usuario](https://docs.microsoft.com/graph/auth-v2-user).
1. [Errores de consentimiento del](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)usuario: en este artículo se analizan los errores que pueden producirse durante el proceso de consentimiento de una aplicación. Si está solucionando mensajes de consentimiento inesperados que no contienen mensajes de error, vea [Escenarios](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)de autenticación para Azure AD .