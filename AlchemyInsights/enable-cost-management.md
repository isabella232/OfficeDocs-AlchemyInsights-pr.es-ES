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
# <a name="enable-cost-management"></a>Habilitar la administración de costos

**¿Qué significa "costos deshabilitados para la organización"?**

Las organizaciones que usan el contrato Enterprise (EA) o las cuentas de acuerdo de cliente de Microsoft (MCA) pueden deshabilitar el acceso a la información de costes y a la información de precios.

Después de iniciar sesión en Azure portal, pueden usar las API de facturación para obtener facturas mediante programación (una vez que se hayan elegido) y los detalles de uso.

**Cómo permitir que otros usuarios obtengan acceso a facturas**

1. Vaya a la **hoja suscripciones** en Azure portal.
2. Seleccione **facturas** y, a continuación, **acceso a facturas**.
3. Active el acceso y, después, guarde los cambios para permitir que los usuarios de roles con ámbito de suscripción puedan descargar facturas.

> [!NOTE]
> El administrador de la cuenta también puede configurar para que las facturas se envíen por correo electrónico. Para obtener más información, consulte [obtener la factura en un correo electrónico](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Cómo agregar usuarios al rol de lector de facturación**

1. Vaya a la **hoja suscripciones** en Azure portal.
2. Seleccione **control de acceso (IAM)** y, a continuación, haga clic en **Agregar**.
3. Elija **lector de facturación** en la página **seleccionar un rol** .
4. Escriba el correo electrónico del usuario que desea invitar y, a continuación, haga clic en **Aceptar** para enviar la invitación.
5. Siga las instrucciones proporcionadas en el correo electrónico invite para iniciar sesión como lector de facturación. Para obtener más información, vea [conceder acceso a la facturación](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Documentos recomendados**

- [Habilitar vistas de DA y AO a través del portal de AE](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Costos incluidos en la administración de costos](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Ofertas admitidas de Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Revisión de costos en análisis de costos](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Proporcionar acceso a la información de facturación](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprobar el acceso a un acuerdo de cliente de Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






