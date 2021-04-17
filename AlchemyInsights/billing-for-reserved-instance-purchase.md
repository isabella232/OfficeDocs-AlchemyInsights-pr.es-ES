---
title: Facturación de compra de instancias reservadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820339"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturación de compra de instancias reservadas

La compra de instancia reservada se carga al método de pago vinculado a la suscripción que selecciones en el momento de la compra. El tipo de suscripción debe ser un contrato de empresa (número de oferta: MS-AZR-0017P), Pay-As-You-Go (número de oferta: MS-AZR-0003P), Contrato de cliente de Microsoft o CSP.

- Para una suscripción empresarial, los cargos se descuentan del saldo de compromiso monetario de la inscripción o se cobran como excesos
- Para la suscripción de pago por uso, los cargos se facturan a la tarjeta de crédito o al método de pago de factura en la suscripción

**Cancelación de reserva**

- **Autoservicio:** Puede cancelar o intercambiar una instancia reservada usted mismo con [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Seleccione la reserva y haga clic en Reembolso o Cambio. Tenga en cuenta que debe tener acceso de propietario en el pedido de reserva para cambiar o reembolsar. El acceso a solo la reserva no le permitirá continuar con el reembolso o el intercambio. Solicitar al propietario de la orden de reserva que le dé acceso al propietario a la Orden de reserva
- **Directiva de Exchange:** Puede cambiar una reserva por otra del mismo tipo: no hay **penalizaciones** en el intercambio de reservas. El compromiso total con la nueva reserva debe ser mayor que la suma del importe de reembolso de la reserva intercambiada y los pagos mensuales futuros (si procede)
- **Directiva de reembolso:** La suma del reembolso y los pagos futuros cancelados no pueden superar los 50 000 USD en una ventana de 12 meses. Actualmente no **estamos cobrando ninguna penalización por** reembolsos, pero podría cobrarla en reembolsos futuros

**Excepciones:** La capacidad de intercambio y cancelación de autoservicio no está disponible para clientes de administración pública Contrato Enterprise ee. UU.

- **El soporte técnico de API/PS/CLI** no está disponible para cancelaciones y reembolsos de intercambios de autoservicio y [reembolsos para reservas de Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- La funcionalidad de intercambio y cancelación de autoservicio no está disponible para los clientes Contrato Enterprise administración pública. Se admiten otros tipos de suscripción de Us Government, como Pay-As-You-Go y CSP.

Más información : [Cómo se procesan las](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) transacciones de devolución y cambio Obtenga más información: Directivas de [exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) y reembolso Otras preguntas: Visitar documentos de [instancia reservada](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange una instancia reservada existente (autoservicio)**

Puede cambiar una reserva por otra reserva del mismo tipo. También puedes reembolsar una reserva, hasta 50 000 USD al año, si ya no la necesitas. La funcionalidad de intercambio y cancelación de autoservicio no está disponible para los clientes Contrato Enterprise administración pública. Se admiten otros tipos de suscripción de Us Government, como Pay-As-You-Go y CSP. Debe tener acceso de propietario en el pedido de reserva para intercambiar o reembolsar una reserva existente.

Los pasos siguientes guiarán el procedimiento para completar la transacción

1.Inicie sesión en [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Seleccione las reservas que desea reembolsar y haga clic en **Exchange** 2.Seleccione el producto de máquina virtual que desea comprar y escriba una cantidad. Asegúrese de que el nuevo total de compra sea mayor que el total devuelto [Determine el tamaño correcto antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Revisar y completar la transacción

**Reembolso de una instancia reservada**

Para reembolsar una reserva, vaya a **Detalles de la reserva** y haga clic en **Reembolso**

**Reembolso prorrateada:**

**Ejemplos de requisitos mínimos** y pro-ración para reembolso y cambio Ejemplo de reserva inicial:

- Comprar una instancia reservada de un año por 120 $ el 1 de enero
- El 7 de abril quieres reembolsar o cambiar esta reserva
- Dado que la reserva ha estado en directo durante 97 días, recibirá (1-97/365) * $120 de vuelta. (es decir, 88,1 $). Actualmente no hay ninguna penalización en los reembolsos
- Si se intercambia, la nueva compra debe ser mayor que $88,1
- No hay ninguna penalización en los reembolsos actualmente

**Ejemplo de reserva del plan de facturación:**

- Comprar una instancia reservada de un año por $10 al mes
- El 7 de abril quieres reembolsar o cambiar esta reserva
- Dado que el último pago se produjo 7 días, recibirá (1-7/31) * $10 de vuelta. (es decir, 7,74 $)
- Los pagos futuros cancelados son de 80 $. Actualmente no hay ninguna penalización en los reembolsos
- Esta cancelación deducirá $87,74 del límite de reembolso de $50,000
- Si se intercambia, el valor total de la nueva compra debe ser mayor que $87,74

**No se puede ver la factura del último período de facturación**

Algunos posibles motivos por los que es posible que no vea una factura:

- Tiene un importe de crédito mensual con la suscripción que no superó o tiene una versión de prueba gratuita. Una factura solo se genera cuando debe dinero
- Son menos de 30 días desde el día en que se suscribió a Azure
- La factura aún no se ha generado. Esperar hasta el final del período de facturación
- Si no es el administrador de la cuenta, es posible que las facturas anteriores no estén disponibles.

**Descargar la factura de Azure Portal (.pdf)**

- Seleccione su suscripción en la página [Suscripciones](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) de Azure Portal como usuario con [acceso a facturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Seleccionar **facturas**
- Haga clic en **Descargar factura** para ver una copia de su factura en PDF. Si dice **No disponible**, vea ¿Por qué no veo una factura para el último período de [facturación?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Recibir la factura por correo electrónico (.pdf)**

- Selecciona tu suscripción en la [página Suscripciones.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Haga **clic en Facturas** y, a continuación, envíe un correo electrónico a mi factura
- Haga **clic en Participar** y acepte los términos. Tendrá que participar en cada suscripción que tenga

Nota: Si no recibe un correo electrónico después de seguir los pasos, asegúrese de que su dirección de correo electrónico sea correcta en las preferencias de [comunicación de su perfil](https://account.windowsazure.com/profile)

**Descargar los datos de uso desde Azure Portal**

- Inicie sesión en [el Centro de cuentas de Azure](https://account.windowsazure.com/Subscriptions) como administrador de [cuentas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Seleccione la suscripción para la que desea la factura y la información de uso
- Seleccionar **historial de facturación**
- Seleccione **Ver instrucción actual** para ver una estimación de los cargos en el momento en que se generó la estimación
- Seleccione **Descargar uso** para descargar los datos de uso diario como un archivo CSV. Si ve dos versiones disponibles, descargue la versión 2

Otras preguntas: [Visitar documentos de instancia reservada](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos recomendados**

- [Conceptos básicos de facturación](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender cómo se aplica el descuento de instancia reservada](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Descargar o ver la factura de facturación de Azure y los datos de uso diario](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender cómo se aplica el descuento de instancia reservada](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender el uso de instancias reservadas para la suscripción de pago por uso](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprender el uso de instancias reservadas para la inscripción de enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Los costos de software de Windows no se incluyen con instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instancias reservadas en el programa Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)