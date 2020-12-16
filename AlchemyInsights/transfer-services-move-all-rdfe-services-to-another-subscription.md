---
title: 'Transfer Services: mueve todos los servicios RDFE a otra suscripción'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681508"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="dd3ba-102">Transfer Services: mueve todos los servicios RDFE a otra suscripción</span><span class="sxs-lookup"><span data-stu-id="dd3ba-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="dd3ba-103">**Mover recursos**</span><span class="sxs-lookup"><span data-stu-id="dd3ba-103">**Move resources**</span></span>

<span data-ttu-id="dd3ba-104">Los recursos de Azure se pueden mover a otro grupo de recursos o suscripción de Azure en la misma suscripción mediante Azure portal, Azure PowerShell, Azure CLI o la API de REST para mover recursos.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="dd3ba-105">Para poder mover recursos, vea:</span><span class="sxs-lookup"><span data-stu-id="dd3ba-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="dd3ba-106">Lista de comprobación antes de mover recursos</span><span class="sxs-lookup"><span data-stu-id="dd3ba-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="dd3ba-107">Servicios que se pueden mover</span><span class="sxs-lookup"><span data-stu-id="dd3ba-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="dd3ba-108">Cómo validar el movimiento</span><span class="sxs-lookup"><span data-stu-id="dd3ba-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="dd3ba-109">Mover la guía para los servicios</span><span class="sxs-lookup"><span data-stu-id="dd3ba-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="dd3ba-110">Para mover los recursos existentes a otro grupo de recursos o suscripción, puede usar:</span><span class="sxs-lookup"><span data-stu-id="dd3ba-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="dd3ba-111">Portal de Azure</span><span class="sxs-lookup"><span data-stu-id="dd3ba-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="dd3ba-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="dd3ba-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="dd3ba-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dd3ba-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="dd3ba-114">API de REST</span><span class="sxs-lookup"><span data-stu-id="dd3ba-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="dd3ba-115">Tutorial: [mover recursos de Azure a otro grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="dd3ba-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="dd3ba-116">**Solucionar errores con Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="dd3ba-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="dd3ba-117">Consulte los artículos siguientes para obtener información sobre algunos errores comunes de implementación de Azure y recibir información para resolverlos.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="dd3ba-118">Si no encuentra el código de error del error de implementación, vea [Buscar Código de error](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="dd3ba-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="dd3ba-119">Solucionar errores de implementación</span><span class="sxs-lookup"><span data-stu-id="dd3ba-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="dd3ba-120">Solucionar problemas al mover recursos de Azure a un nuevo grupo de recursos o suscripción</span><span class="sxs-lookup"><span data-stu-id="dd3ba-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="dd3ba-121">Tenga en cuenta que si desea actualizar su suscripción a Azure, como cambiar de la versión gratuita a la de pago por su cuenta, tendrá que convertir su suscripción.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="dd3ba-122">Para actualizar una prueba gratuita, consulte [upgrade Your Free Trial o Microsoft Imagine Azure Inscription to pay-as-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="dd3ba-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="dd3ba-123">Para cambiar una cuenta de pago por su cuenta, consulta [cambiar la suscripción de pago por su Azure pago por su acceso a una oferta diferente](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="dd3ba-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="dd3ba-124">**Para agregar o asociar una suscripción de Azure a su inquilino de Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="dd3ba-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="dd3ba-125">Inicie sesión y seleccione la suscripción que desea usar en la [Página suscripciones de Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="dd3ba-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="dd3ba-126">Seleccione **cambiar directorio**.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="dd3ba-127">Revise las advertencias que aparecen y, a continuación, seleccione **cambiar**.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="dd3ba-128">El directorio se cambia para la suscripción y recibirá un mensaje de confirmación.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="dd3ba-129">Use el conmutador de *directorio* para ir a su nuevo directorio.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="dd3ba-130">Puede tardar hasta 10 minutos para que todo se muestre correctamente.</span><span class="sxs-lookup"><span data-stu-id="dd3ba-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="dd3ba-131">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="dd3ba-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="dd3ba-132">Transferir la propiedad de una suscripción de Azure</span><span class="sxs-lookup"><span data-stu-id="dd3ba-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="dd3ba-133">Mover recursos a un nuevo grupo de recursos o suscripción</span><span class="sxs-lookup"><span data-stu-id="dd3ba-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="dd3ba-134">Administrar recursos con Azure portal</span><span class="sxs-lookup"><span data-stu-id="dd3ba-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
