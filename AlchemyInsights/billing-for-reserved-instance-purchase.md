---
title: Facturación de compra de instancias reservadas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816035"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturación de compra de instancias reservadas

La compra de la instancia reservada se cargará en el método de pago vinculado a la suscripción seleccionada en el momento de la compra. El tipo de suscripción debe ser un contrato Enterprise (número de oferta: MS-AZR-0017P), pago por uso (número de oferta: MS-AZR-0003P), el Contrato de cliente de Microsoft o el Proveedor de soluciones en la nube de Microsoft.

- En el caso de una suscripción de Enterprise, los cobros se deducirán del saldo del compromiso monetario de la inscripción o se le cobrará como excedente
- Para las suscripciones de pago por uso, los cobros se facturarán al método de pago mediante tarjeta de crédito o factura de la suscripción.

**Cancelar reserva**

- **Autoservicio:** usted mismo puede cancelar o intercambiar una instancia reservada mediante el [portal de Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Seleccione la reserva y haga clic en reembolso o intercambio. Tenga en cuenta que debe tener acceso de propietario al Pedido de reserva para hacer el intercambio o reembolso. El acceso solo a la Reserva no le permitirá continuar con el reembolso o intercambio. Pida al propietario del Pedido de reserva que le proporcione acceso de propietario.
- **Directiva de intercambio:** es posible intercambiar una reserva por otra del mismo tipo. No hay **ninguna sanción** sobre el intercambio de reservas. La oferta total con la nueva reserva debe ser mayor que la suma del importe de reembolso de la reserva intercambiada y los pagos mensuales futuros (si corresponde).
- **Directiva de reembolso:** la suma del reembolso y los pagos futuros cancelados no puede superar los $50.000 USD en un período de 12 meses. **Actualmente no realizamos cargos por penalización** sobre reembolsos, pero podrían realizarse sobre futuros reembolsos.

**Excepciones:** La capacidad de intercambio y cancelación de autoservicio no está disponible para los clientes del Contrato Enterprise de US Government

- El soporte de **API / PS / CLI** no está disponible para la cancelación y el reembolso [Intercambios y reembolsos de autoservicio para las reservas de Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- La capacidad de intercambio y cancelación de autoservicio no está disponible para los clientes del Contrato Enterprise de US Government Se admiten otros tipos de suscripciones de US Government, incluidos el Pago por uso y el CSP.

Obtenga más información: [cómo se procesan las transacciones de devolución y de Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) : más información sobre [las directivas de reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) y de reembolso otras preguntas: [visite la instancia reservada docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Intercambiar una instancia reservada existente (autoservicio)**

Puede intercambiar una reserva por otra del mismo tipo. También puede reembolsar una reserva, de hasta $50.000 USD por año, si ya no la necesita. La capacidad de intercambio y cancelación de autoservicio no está disponible para los clientes del Contrato Enterprise de US Government Se admiten otros tipos de suscripciones de US Government, incluidos el Pago por uso y el CSP. Debe tener acceso de propietario al Pedido de reserva para intercambiar o reembolsar una reserva existente.

Los siguientes pasos le guiarán sobre el procedimiento para completar la transacción

1. Inicie sesión en el [portal de Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Seleccione las reservas que desea reembolsar y haga clic en **Exchange** 2. Seleccione el producto de la máquina virtual que desea comprar y escriba una cantidad. Asegúrese de que el nuevo total de compra es mayor que el total devuelto: [determine el tamaño correcto antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. revisar y completar la transacción

**Reembolso de una instancia reservada**

Para reembolsar una reserva, vaya a **Detalles de reserva** y haga clic en **Reembolso**

**Reembolso prorrateado:**

**Pro-ración y ejemplos de requisitos mínimos para reembolso e intercambio** Ejemplo de reserva de la parte superior:

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

**No se puede ver la factura del último período de facturación**

Algunas posibles razones por las que podría no ver una factura:

- Tiene una cantidad de crédito mensual con su suscripción que no ha superado o tiene una versión de prueba gratuita. Solo se genera una factura cuando se le debe dinero.
- Es menos de 30 días a partir del día en que se suscribió a Azure.
- La factura aún no se ha generado. Esperar hasta el final del período de facturación
- Si no es el administrador de la cuenta, es posible que no haya facturas más antiguas disponibles

**Descargar la factura del portal de Azure (. pdf)**

- Seleccione su suscripción en la página [suscripciones](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) de Azure portal como [usuario con acceso a las facturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support) .
- Seleccionar **facturas**
- Haga clic en **Descargar factura** para ver una copia de su factura PDF. Si **no está disponible** , consulte [¿por qué no veo una factura para el último período de facturación?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Recibir la factura por correo electrónico (. pdf)**

- Seleccione su suscripción en la página [suscripciones](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Haga clic en **facturas** , enviar por correo electrónico mi factura
- Haga clic en **participar** y acepte los términos. Tendrá que optar por todas las suscripciones que posea

Nota: Si no recibe un correo electrónico después de seguir los pasos, asegúrese de que su dirección de correo electrónico es correcta en las [preferencias de comunicación de su perfil](https://account.windowsazure.com/profile) .

**Descargar los datos de uso desde Azure portal**

- Inicie sesión en el [centro de cuentas de Azure](https://account.windowsazure.com/Subscriptions) como administrador de la [cuenta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Seleccione la suscripción para la que desea la información de factura y uso
- Seleccionar **historial de facturación**
- Seleccione **Ver instrucción actual** para ver una estimación de los cargos en el momento en que se generó la estimación.
- Seleccione **Descargar uso** para descargar los datos de uso diario como un archivo CSV. Si ve dos versiones disponibles, descargue la versión 2.

Otras preguntas: [Visite los documentos sobre instancias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos recomendados**

- [Conceptos básicos de facturación](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender cómo se aplica el descuento de instancia reservada](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Descargar o ver la factura de facturación de Azure y los datos de uso diarios](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender cómo se aplica el descuento de instancia reservada](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender el uso de instancias reservadas para la suscripción de pago por uso](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Descripción del uso de instancias reservadas para la inscripción de empresa](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Costos de software de Windows no incluidos en las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instancias reservadas en el programa de proveedor de soluciones de nube (CSP) central de asociados](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)