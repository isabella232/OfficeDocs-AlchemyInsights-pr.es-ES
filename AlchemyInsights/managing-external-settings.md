---
title: Administrar la configuración externa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282862"
---
# <a name="managing-external-settings"></a><span data-ttu-id="7105d-102">Administrar la configuración externa</span><span class="sxs-lookup"><span data-stu-id="7105d-102">Managing External Settings</span></span>

<span data-ttu-id="7105d-103">**Anuncio**</span><span class="sxs-lookup"><span data-stu-id="7105d-103">**Announcement**</span></span>

- <span data-ttu-id="7105d-104">[Desuso del soporte de inicio de sesión de WebView de Google a partir del 4 de enero de 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="7105d-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="7105d-105">Siga las instrucciones de pruebas de compatibilidad de Google para comprobar si las aplicaciones se ven afectadas.</span><span class="sxs-lookup"><span data-stu-id="7105d-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="7105d-106">Asegúrese de usar la vista web del sistema o el explorador del sistema al iniciar la sesión de los usuarios con cuentas de Google de consumidor.</span><span class="sxs-lookup"><span data-stu-id="7105d-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="7105d-107">**Administrar la configuración de invitación**</span><span class="sxs-lookup"><span data-stu-id="7105d-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="7105d-108">Confirme que ha [configurado los ajustes de colaboración externa](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) para permitir a las personas apropiadas enviar invitaciones.</span><span class="sxs-lookup"><span data-stu-id="7105d-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="7105d-109">**Administrar permisos de acceso de usuarios invitados**</span><span class="sxs-lookup"><span data-stu-id="7105d-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="7105d-110">Los administradores globales pueden administrar los permisos de acceso de invitado en el directorio a través de Azure Portal configurando los permisos de acceso de invitado en la página Configuración de colaboración externa.</span><span class="sxs-lookup"><span data-stu-id="7105d-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="7105d-111">[Obtenga más información esta configuración](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="7105d-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="7105d-112">Si desea que los invitados accedan a aplicaciones como Teams o SharePoint, confirme que ha configurado esas aplicaciones para permitir el acceso de invitado.</span><span class="sxs-lookup"><span data-stu-id="7105d-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="7105d-113">Obtenga más información sobre la [Configuración de Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) y [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="7105d-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="7105d-114">**Configurar invitaciones:**</span><span class="sxs-lookup"><span data-stu-id="7105d-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="7105d-115">Habilitar la colaboración externa B2B y gestionar quién puede invitar a los invitados</span><span class="sxs-lookup"><span data-stu-id="7105d-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="7105d-116">Permitir o bloquear invitaciones a usuarios de organizaciones específicas</span><span class="sxs-lookup"><span data-stu-id="7105d-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="7105d-117">**Configurar proveedores de identidades permitidos:**</span><span class="sxs-lookup"><span data-stu-id="7105d-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="7105d-118">Federación de Google</span><span class="sxs-lookup"><span data-stu-id="7105d-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="7105d-119">Federación directa</span><span class="sxs-lookup"><span data-stu-id="7105d-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="7105d-120">Autenticación de código de acceso de un solo uso de correo electrónico</span><span class="sxs-lookup"><span data-stu-id="7105d-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
