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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897759"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="c33bf-102">Solucionar problemas de consentimiento del usuario</span><span class="sxs-lookup"><span data-stu-id="c33bf-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="c33bf-103">Puede configurar cómo los usuarios finales consienten las aplicaciones a través de Azure Portal o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c33bf-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="c33bf-104">Consulta [la configuración de consentimiento del usuario](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="c33bf-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="c33bf-105">Un administrador también puede usar la API de [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para conceder permisos delegados en nombre de un solo usuario.</span><span class="sxs-lookup"><span data-stu-id="c33bf-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="c33bf-106">Para obtener más información, vea [Obtener acceso en nombre de un usuario.](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="c33bf-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="c33bf-107">[Errores de consentimiento del](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)usuario: en este artículo se analizan los errores que pueden producirse durante el proceso de consentimiento de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="c33bf-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="c33bf-108">Si está solucionando problemas de mensajes de consentimiento inesperados que no contienen ningún mensaje de error, vea Escenarios de autenticación [para Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="c33bf-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>