---
title: Habilitar la administración de costos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599084"
---
# <a name="enable-cost-management"></a><span data-ttu-id="fb093-102">Habilitar la administración de costos</span><span class="sxs-lookup"><span data-stu-id="fb093-102">Enable cost management</span></span>

<span data-ttu-id="fb093-103">**¿Qué significa "costos deshabilitados para la organización"?**</span><span class="sxs-lookup"><span data-stu-id="fb093-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="fb093-104">Las organizaciones que usan el contrato Enterprise (EA) o las cuentas de acuerdo de cliente de Microsoft (MCA) pueden deshabilitar el acceso a la información de costes y a la información de precios.</span><span class="sxs-lookup"><span data-stu-id="fb093-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="fb093-105">Después de iniciar sesión en Azure portal, pueden usar las API de facturación para obtener facturas mediante programación (una vez que se hayan elegido) y los detalles de uso.</span><span class="sxs-lookup"><span data-stu-id="fb093-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="fb093-106">**Cómo permitir que otros usuarios obtengan acceso a facturas**</span><span class="sxs-lookup"><span data-stu-id="fb093-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="fb093-107">Vaya a la **hoja suscripciones** en Azure portal.</span><span class="sxs-lookup"><span data-stu-id="fb093-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="fb093-108">Seleccione **facturas** y, a continuación, **acceso a facturas**.</span><span class="sxs-lookup"><span data-stu-id="fb093-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="fb093-109">Active el acceso y, después, guarde los cambios para permitir que los usuarios de roles con ámbito de suscripción puedan descargar facturas.</span><span class="sxs-lookup"><span data-stu-id="fb093-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="fb093-110">El administrador de la cuenta también puede configurar para que las facturas se envíen por correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="fb093-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="fb093-111">Para obtener más información, consulte [obtener la factura en un correo electrónico](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="fb093-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="fb093-112">**Cómo agregar usuarios al rol de lector de facturación**</span><span class="sxs-lookup"><span data-stu-id="fb093-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="fb093-113">Vaya a la **hoja suscripciones** en Azure portal.</span><span class="sxs-lookup"><span data-stu-id="fb093-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="fb093-114">Seleccione **control de acceso (IAM)** y, a continuación, haga clic en **Agregar**.</span><span class="sxs-lookup"><span data-stu-id="fb093-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="fb093-115">Elija **lector de facturación** en la página **seleccionar un rol** .</span><span class="sxs-lookup"><span data-stu-id="fb093-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="fb093-116">Escriba el correo electrónico del usuario que desea invitar y, a continuación, haga clic en **Aceptar** para enviar la invitación.</span><span class="sxs-lookup"><span data-stu-id="fb093-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="fb093-117">Siga las instrucciones proporcionadas en el correo electrónico invite para iniciar sesión como lector de facturación.</span><span class="sxs-lookup"><span data-stu-id="fb093-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="fb093-118">Para obtener más información, vea [conceder acceso a la facturación](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="fb093-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="fb093-119">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="fb093-119">**Recommended documents**</span></span>

- [<span data-ttu-id="fb093-120">Habilitar vistas de DA y AO a través del portal de AE</span><span class="sxs-lookup"><span data-stu-id="fb093-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="fb093-121">Costos incluidos en la administración de costos</span><span class="sxs-lookup"><span data-stu-id="fb093-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="fb093-122">Ofertas admitidas de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="fb093-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="fb093-123">Revisión de costos en análisis de costos</span><span class="sxs-lookup"><span data-stu-id="fb093-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="fb093-124">Proporcionar acceso a la información de facturación</span><span class="sxs-lookup"><span data-stu-id="fb093-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="fb093-125">Comprobar el acceso a un acuerdo de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="fb093-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






