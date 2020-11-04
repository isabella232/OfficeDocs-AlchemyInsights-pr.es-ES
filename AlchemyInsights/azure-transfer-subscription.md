---
title: Transferir la propiedad de facturación de Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840636"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="ba3bb-102">Transferir la propiedad de facturación de Azure</span><span class="sxs-lookup"><span data-stu-id="ba3bb-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="ba3bb-103">Inicie sesión en el [portal de Azure](https://portal.azure.com/) como administrador de la cuenta de facturación que tiene la suscripción que quiere transferir.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="ba3bb-104">Si no está seguro de si es el administrador, o si necesita determinar quién es, vea [Determinar el administrador de facturación de la cuenta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="ba3bb-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="ba3bb-105">Buscar en **Administración de costos + facturación**.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="ba3bb-106">Seleccione **Suscripciones** en el panel izquierdo.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="ba3bb-107">Según el acceso, es posible que tenga que seleccionar un ámbito de facturación y, a continuación, las **Suscripciones** o las **Suscripciones de Azure**.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="ba3bb-108">Seleccione **Transferir propiedad de facturación** para la suscripción que desea transferir</span><span class="sxs-lookup"><span data-stu-id="ba3bb-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="ba3bb-109">Escriba la dirección de correo electrónico de un usuario que sea administrador de facturación de la cuenta que será el nuevo propietario de la suscripción y, a continuación, seleccione **enviar solicitud de transferencia**</span><span class="sxs-lookup"><span data-stu-id="ba3bb-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="ba3bb-110">El usuario recibe un correo electrónico con instrucciones para revisar su solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="ba3bb-111">Para aprobar la solicitud de transferencia, el usuario debe seleccionar el vínculo en el mensaje de correo electrónico y siga las instrucciones.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="ba3bb-112">**Nota** : si se transfiere la propiedad de facturación de su suscripción a una cuenta de usuario en otro espacio empresarial de Azure AD, todas las asignaciones del [control de acceso basado en roles (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para administrar los recursos de la suscripción se eliminan de forma permanente.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="ba3bb-113">Solo el nuevo propietario tendrá acceso para administrar los recursos de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="ba3bb-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="ba3bb-114">Para obtener más información, vea [Transferir la suscripción a un usuario en otro espacio empresarial de Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ba3bb-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ba3bb-115">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="ba3bb-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="ba3bb-116">Transferir la propiedad de facturación de una suscripción de Azure a otra cuenta</span><span class="sxs-lookup"><span data-stu-id="ba3bb-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="ba3bb-117">Acerca de la transferencia de la propiedad de facturación para una suscripción de Azure</span><span class="sxs-lookup"><span data-stu-id="ba3bb-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="ba3bb-118">Transferencia de Visual Studio, Microsoft Partner Network (MPN) y Pay a medida que se dirigen las suscripciones de desarrollo y pruebas</span><span class="sxs-lookup"><span data-stu-id="ba3bb-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="ba3bb-119">Preguntas más frecuentes sobre la transferencia de propiedad</span><span class="sxs-lookup"><span data-stu-id="ba3bb-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="ba3bb-120">Solucionar problemas de transferencia de propiedad</span><span class="sxs-lookup"><span data-stu-id="ba3bb-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
