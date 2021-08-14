---
title: 'Transferir servicios: mover todos los servicios RDFE a otra suscripción'
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940108"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transferir servicios: mover todos los servicios RDFE a otra suscripción

**Mover recursos**

Los recursos de Azure se pueden mover a otro grupo de recursos o suscripción de Azure en la misma suscripción mediante Azure Portal, Azure PowerShell, CLI de Azure o la API de REST para mover recursos.

Antes de poder mover recursos, vea:

- [Lista de comprobación antes de mover recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servicios que se pueden mover](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cómo validar el movimiento](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Instrucciones de movimiento para servicios](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Para mover los recursos existentes a otro grupo de recursos o suscripción, puede usar:

- [<mrk mtype="seg" mid="167">Portal de Azure</mrk>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API de REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [Mover recursos de Azure a otro grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Solucionar errores con Azure Resource Manager**

Consulte los artículos siguientes para obtener información sobre algunos errores comunes de implementación de Azure y recibir información para resolverlos. Si no encuentra el código de error para el error de implementación, vea [Buscar código de error](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Solucionar errores de implementación](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Solucionar problemas al mover recursos de Azure a un nuevo grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Ten en cuenta que si quieres actualizar la suscripción de Azure, como cambiar de gratis a pagar por uso, deberás convertir la suscripción.

- Para actualizar una versión de prueba gratuita, consulte [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Para cambiar una cuenta de pago por uso, vea Cambiar la suscripción de [Azure Pay-As-You-Go a una oferta diferente.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Para agregar o asociar una suscripción de Azure a su Azure Active Directory inquilino:**

1. Inicie sesión y seleccione la suscripción que desea usar en la página [Suscripciones de Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Seleccione **Cambiar directorio**.
3. Revise las advertencias que aparezcan y, a continuación, **seleccione Cambiar**.
4. El directorio se cambia para la suscripción y recibirá un mensaje de éxito.
5. Use el *modificador de* directorio para ir al nuevo directorio. Todo puede tardar hasta 10 minutos en aparecer correctamente.

**Documentos recomendados**

- [Transferir la propiedad de una suscripción de Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mover recursos al nuevo grupo de recursos o suscripción](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Administrar recursos con Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
