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
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003586"
---
# <a name="enable-cost-management"></a>Habilitar la administración de costos

**¿Qué significa "los costos están deshabilitados para su organización"?**

Las organizaciones que usan Enterprise Agreement (EA) o cuentas de Contrato de cliente de Microsoft (MCA) pueden deshabilitar el acceso a información de costos e información de precios.

Después de iniciar sesión en Azure Portal, pueden usar las API de facturación para obtener mediante programación facturas (una vez que se han optado) y detalles de uso.

**Cómo permitir que usuarios adicionales accedan a facturas**

1. Vaya a **La hoja Suscripciones** en Azure Portal.
2. Seleccione **Facturas y,** a **continuación, Acceso a facturas**.
3. Activa el acceso, seguido de guardar los cambios, para permitir que los usuarios con roles de ámbito de suscripción descarguen facturas.

> [!NOTE]
> El administrador de la cuenta también puede configurar para que las facturas se envíen por correo electrónico. Para obtener más información, consulte [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Cómo agregar usuarios al rol Lector de facturación**

1. Vaya a **La hoja Suscripciones** en Azure Portal.
2. Seleccione **Control de acceso (IAM)** y, a continuación, haga clic en **Agregar**.
3. Elija **Lector de facturación** en **la página Seleccionar un rol.**
4. Escriba el correo electrónico del usuario que desea invitar y, a continuación, haga clic en **Aceptar** para enviar la invitación.
5. Siga las instrucciones proporcionadas en el correo electrónico de invitación para iniciar sesión como lector de facturación. Para obtener más información, vea [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Documentos recomendados**

- [Habilitar vistas de DA y AO a través del portal de EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Costos incluidos en Administración de costos](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Ofertas Microsoft Azure compatibles](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Revisar los costos en el análisis de costos](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Proporcionar acceso a la información de facturación](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprobar el acceso a un Contrato de cliente de Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






