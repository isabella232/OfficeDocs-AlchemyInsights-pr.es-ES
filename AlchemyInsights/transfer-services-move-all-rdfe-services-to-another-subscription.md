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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services: mueve todos los servicios RDFE a otra suscripción

**Mover recursos**

Los recursos de Azure se pueden mover a otro grupo de recursos o suscripción de Azure en la misma suscripción mediante Azure portal, Azure PowerShell, Azure CLI o la API de REST para mover recursos.

Para poder mover recursos, vea:

- [Lista de comprobación antes de mover recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servicios que se pueden mover](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cómo validar el movimiento](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Mover la guía para los servicios](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Para mover los recursos existentes a otro grupo de recursos o suscripción, puede usar:

- [Portal de Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API de REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [mover recursos de Azure a otro grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Solucionar errores con Azure Resource Manager**

Consulte los artículos siguientes para obtener información sobre algunos errores comunes de implementación de Azure y recibir información para resolverlos. Si no encuentra el código de error del error de implementación, vea [Buscar Código de error](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Solucionar errores de implementación](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Solucionar problemas al mover recursos de Azure a un nuevo grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Tenga en cuenta que si desea actualizar su suscripción a Azure, como cambiar de la versión gratuita a la de pago por su cuenta, tendrá que convertir su suscripción.

- Para actualizar una prueba gratuita, consulte [upgrade Your Free Trial o Microsoft Imagine Azure Inscription to pay-as-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Para cambiar una cuenta de pago por su cuenta, consulta [cambiar la suscripción de pago por su Azure pago por su acceso a una oferta diferente](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Para agregar o asociar una suscripción de Azure a su inquilino de Azure Active Directory:**

1. Inicie sesión y seleccione la suscripción que desea usar en la [Página suscripciones de Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Seleccione **cambiar directorio**.
3. Revise las advertencias que aparecen y, a continuación, seleccione **cambiar**.
4. El directorio se cambia para la suscripción y recibirá un mensaje de confirmación.
5. Use el conmutador de *directorio* para ir a su nuevo directorio. Puede tardar hasta 10 minutos para que todo se muestre correctamente.

**Documentos recomendados**

- [Transferir la propiedad de una suscripción de Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mover recursos a un nuevo grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Administrar recursos con Azure portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
