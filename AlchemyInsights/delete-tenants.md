---
title: Eliminar espacio empresarial
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477704"
---
# <a name="delete-tenant"></a><span data-ttu-id="7f500-102">Eliminar espacio empresarial</span><span class="sxs-lookup"><span data-stu-id="7f500-102">Delete tenant</span></span>

<span data-ttu-id="7f500-103">Para eliminar Azure AD, asegúrese de lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="7f500-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="7f500-104">Es un administrador global en el directorio.</span><span class="sxs-lookup"><span data-stu-id="7f500-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="7f500-105">NO ha iniciado sesión con una cuenta que tiene el directorio predeterminado, por ejemplo, contoso.onmicrosoft.com, en la cuenta firmada, como admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="7f500-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="7f500-106">Quite todas las aplicaciones activas del directorio antes de la eliminación.</span><span class="sxs-lookup"><span data-stu-id="7f500-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="7f500-107">Para quitar las aplicaciones activas, vaya a registros de aplicaciones y quite las aplicaciones existentes.</span><span class="sxs-lookup"><span data-stu-id="7f500-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="7f500-108">No hay suscripciones activas para los servicios en línea de Microsoft, como Microsoft Azure, Office 365 o Azure AD Premium asociados en el directorio.</span><span class="sxs-lookup"><span data-stu-id="7f500-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="7f500-109">Transferir sus suscripciones o acelerar la cancelación de suscripciones activas a través de la facturación y soporte de Azure.</span><span class="sxs-lookup"><span data-stu-id="7f500-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="7f500-110">Obtenga más información sobre cómo cancelar las suscripciones de Office 365 y Azure.</span><span class="sxs-lookup"><span data-stu-id="7f500-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="7f500-111">Para obtener instrucciones sobre cómo asociar o agregar una suscripción existente a un inquilino, vea [Associate or Add a Azure Inscription to your Azure ad tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="7f500-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="7f500-112">No hay ninguna licencia activa.</span><span class="sxs-lookup"><span data-stu-id="7f500-112">There are no Active license.</span></span> <span data-ttu-id="7f500-113">Para quitar licencias, consulte [How to Remove subscription to Remove License](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="7f500-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="7f500-114">No hay otros usuarios activos en el directorio, aparte del administrador global, al intentar eliminar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f500-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="7f500-115">Quite los demás usuarios activos y se deberán quitar todas las dependencias de un nombre de dominio personalizado en el inquilino, como los usuarios creados con admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="7f500-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="7f500-116">Para obtener más información acerca de los pasos para:</span><span class="sxs-lookup"><span data-stu-id="7f500-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="7f500-117">Eliminar "Azure Active Directory" o "suscripción", vea [eliminar Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="7f500-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="7f500-118">Quitar aplicaciones del directorio, vea [quitar aplicaciones](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="7f500-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
