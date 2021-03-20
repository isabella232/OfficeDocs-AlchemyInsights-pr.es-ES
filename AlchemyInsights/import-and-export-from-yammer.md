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
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898049"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="224af-102">Importación y exportación desde Yammer</span><span class="sxs-lookup"><span data-stu-id="224af-102">Import and export from Yammer</span></span>

<span data-ttu-id="224af-103">**Importación**</span><span class="sxs-lookup"><span data-stu-id="224af-103">**Import**</span></span>

<span data-ttu-id="224af-104">Las opciones de importación de usuarios varían según si la red de Yammer está en [Modo nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) o no.</span><span class="sxs-lookup"><span data-stu-id="224af-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="224af-105">**Modo no nativo**: se puede importar a usuarios a grupos mediante [Añadir desde la Libreta de direcciones](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limitado a 100 usuarios) dentro de la configuración de grupos, o bien a la red a través de [Actualización masiva](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) dentro de Administrador de red.</span><span class="sxs-lookup"><span data-stu-id="224af-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="224af-106">**Modo nativo**: las operaciones de suscripción a grupos y a la red deben realizarse desde el [portal de Administración de Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), el [portal de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) o mediante otra opción de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="224af-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="224af-107">Las redes en Modo nativo ya no tienen acceso a la Actualización masiva y otras funciones heredadas.</span><span class="sxs-lookup"><span data-stu-id="224af-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="224af-108">Yammer nunca fue compatible con la importación de contenido desde el Administrador de red, incluso cuando la característica de Exportación de datos se usó en otra red.</span><span class="sxs-lookup"><span data-stu-id="224af-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="224af-109">Las soluciones de asociados o las API de REST de Yammer pueden volver a publicar el contenido.</span><span class="sxs-lookup"><span data-stu-id="224af-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="224af-110">**Exportación**</span><span class="sxs-lookup"><span data-stu-id="224af-110">**Export**</span></span>

<span data-ttu-id="224af-111">La [Exportación de datos de red dentro del Administrador de red](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permite exportar contenido de redes de Yammer, incluyendo mensajes y archivos.</span><span class="sxs-lookup"><span data-stu-id="224af-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="224af-112">Los archivos adjuntos pueden ser extremadamente grandes y harán que las exportaciones tarden un tiempo considerable en completarse.</span><span class="sxs-lookup"><span data-stu-id="224af-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="224af-113">Recomendamos que las redes activas se exporten utilizando la [API de exportación de datos](https://developer.yammer.com/docs/data-export-api) en partes por día o por semana.</span><span class="sxs-lookup"><span data-stu-id="224af-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="224af-114">El soporte técnico de Microsoft no proporciona scripts personalizados para este propósito.</span><span class="sxs-lookup"><span data-stu-id="224af-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="224af-115">Existe una [exportación de RGPD](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) separada para exportar contenido para un usuario individual.</span><span class="sxs-lookup"><span data-stu-id="224af-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>