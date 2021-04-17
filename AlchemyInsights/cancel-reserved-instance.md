---
title: Cancelar reserva
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819709"
---
# <a name="cancelling-reservation"></a>Cancelar reserva

- **Autoservicio:** usted mismo puede cancelar o intercambiar una instancia reservada mediante el [portal de Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Seleccione la reserva y haga clic en reembolso o intercambio. Tenga en cuenta que debe tener acceso de propietario al Pedido de reserva para hacer el intercambio o reembolso. El acceso solo a la Reserva no le permitirá continuar con el reembolso o intercambio. Pida al propietario del Pedido de reserva que le proporcione acceso de propietario.
- **Directiva de intercambio:** es posible intercambiar una reserva por otra del mismo tipo. No hay **ninguna sanción** sobre el intercambio de reservas. La oferta total con la nueva reserva debe ser mayor que la suma del importe de reembolso de la reserva intercambiada y los pagos mensuales futuros (si corresponde).
- **Directiva de reembolso:** la suma del reembolso y los pagos futuros cancelados no puede superar los $50.000 USD en un período de 12 meses. **Actualmente no realizamos cargos por penalización** sobre reembolsos, pero podrían realizarse sobre futuros reembolsos.  
    **Excepciones:** La capacidad de intercambio y cancelación de autoservicio no está disponible para los clientes del Contrato Enterprise de US Government
- El soporte de **API / PS / CLI** no está disponible para la cancelación y el reembolso [Intercambios y reembolsos de autoservicio para las reservas de Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- La capacidad de intercambio y cancelación de autoservicio no está disponible para los clientes del Contrato Enterprise de US Government Se admiten otros tipos de suscripciones de US Government, incluidos el Pago por uso y el CSP.

Más información : [Cómo se procesan las transacciones de reembolso e intercambio](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Más información : [Directivas de intercambio y reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Otras preguntas: [Visite los documentos sobre instancias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Intercambiar una instancia reservada existente (autoservicio)**

Puede intercambiar una reserva por otra del mismo tipo. También puede reembolsar una reserva, de hasta $50.000 USD por año, si ya no la necesita. La capacidad de intercambio y cancelación de autoservicio no está disponible para los clientes del Contrato Enterprise de US Government Se admiten otros tipos de suscripciones de US Government, incluidos el Pago por uso y el CSP. Debe tener acceso de propietario al Pedido de reserva para intercambiar o reembolsar una reserva existente.

Los siguientes pasos le guiarán sobre el procedimiento para completar la transacción

1. Inicie sesión en el [portal de Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Seleccione las reservas que desea reembolsar y haga clic en **Exchange**
2. Seleccione el producto de VM que desee comprar y escriba una cantidad. Asegúrese de que el total de la nueva compra es superior al total devuelto [Determinar el valor correcto antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Revisar y completar la transacción

**Reembolso de una instancia reservada**

Para reembolsar una reserva, vaya a **Detalles de reserva** y haga clic en **Reembolso**

**Reembolso prorrateado:**

**Ejemplos de prorrateo y requisitos mínimos para reembolsos e intercambios**  
Ejemplo de reserva por adelantado:

- Compra un período de reserva de un año por $120, el 1 de enero.
- El día 7 de abril, quiere que se le reembolse o intercambie esta reserva.
- Como la reserva ha estado activa durante 97 días, recibirá de vuelta el resultado de (1-97/365) multiplicado por $120. (por ejemplo, $88,1). Actualmente, no hay ninguna penalización sobre los reembolsos
- Si hace un intercambio, la nueva compra debe ser mayor de $88,1
- No hay ningún tipo de penalización sobre los reembolsos actualmente.

**Ejemplo de reserva de plan de facturación:**

- Compra un período de reserva de un año por $10 al mes.
- El día 7 de abril, quiere que se le reembolse o intercambie esta reserva.
- Como el último pago ocurrió hace 7 días, recibirá de vuelta el resultado de (1-7/31) multiplicado por $10. (por ejemplo, $7,74).
- Los pagos futuros cancelados corresponden a $80. Actualmente, no hay ninguna penalización sobre los reembolsos
- Esta cancelación deducirá $87,74 de su límite de reembolso de $50.000.
- Si hace un intercambio, el valor total de la nueva compra debe ser mayor que $87,74.

**Documentos recomendados**

- [Cómo se procesan las transacciones de reembolso e intercambio](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Directivas de intercambio y reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)