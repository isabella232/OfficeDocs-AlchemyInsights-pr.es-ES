---
title: ¿Por qué el botón Agregar presupuesto está deshabilitado para mí?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769593"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>¿Por qué el botón Agregar presupuesto está deshabilitado para mí?

Para crear un presupuesto, necesita uno de los siguientes permisos:

- Ámbito de grupo de administración, suscripción y ámbitos de grupo de recursos
- Colaborador de administración de costos
- Owner
- Colaborador
- Solo cliente de empresa: inscripción, Departamento, ámbitos de cuenta
- Administrador de inscripción (establecer el presupuesto en el ámbito de inscripción)
- Administrador de departamento (establecer el presupuesto en el ámbito del Departamento)
- Propietario de la cuenta (establecer el presupuesto en el ámbito de la cuenta)
- Solo acuerdo de cliente moderno: cuenta de facturación, perfil de facturación, ámbitos de la sección de factura
- Creador de la suscripción de Azure

**He creado una cotización cuando el costo del mes actual ya ha superado el presupuesto. ¿Por qué no recibo una alerta?**  
Si ya ha superado un umbral de costo determinado al crear un presupuesto, la alerta no se activará. Una vez que comienza un nuevo ciclo, si infringe el umbral, la alerta se activará.

**¿Cuándo se debe esperar recibir una alerta después de superar uno de los umbrales de alerta presupuestado definidos?**  
Los presupuestos se evalúan cada 4 horas. Los datos de uso tardan un mínimo de 8 horas en llegar al sistema de presupuestos. En este momento, las alertas pueden tardar hasta 12 horas en iniciarse después de superar un umbral.

**¿Por qué el botón fecha de inicio está deshabilitado cuando selecciono un mes o un período de restablecimiento de un mes de facturación?**  
Los presupuestos se alinean con el mes del calendario actual o el período de facturación actual (en caso de que se seleccione mes de facturación). Por lo tanto, rellenaremos este valor por usted de antemano.

**¿Por qué no veo un gráfico de mis costos en la experiencia de creación de presupuestos?**  
Necesitamos un mínimo de 2 meses de datos de costo antes de que podamos representar un gráfico para ayudarle a crear el presupuesto.

**¿Por qué no puedo establecer un presupuesto contra una suscripción que acabo de crear?**  
Después de crear una suscripción, los datos tardan 24-48 horas en procesarse antes de establecer un presupuesto.

**Recursos de la API de presupuesto**

- [Budget API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): proporciona operaciones para crear y actualizar presupuestos. Mediante el uso de la API de presupuestos, puede establecer un umbral de presupuesto y configurar varias alertas para que se activen al enfocar ese umbral. Las alertas pueden desencadenar un correo electrónico o un grupo de acciones de Azure para realizar la automatización. Nota: el filtrado de esta API no se alinea con las dimensiones y el filtrado de la API de consulta.
- [API de presupuestos V2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): cree presupuestos con mayor capacidad de filtrado de costos que v1. El filtrado se alinea con el contrato usado en nuestras API de consulta y dimensiones. Esta es la API de presupuestos recomendados para seguir adelante.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): proporciona operaciones para obtener las dimensiones admitidas para su uso en una variedad de ámbitos. Con la API de dimensiones, puede recuperar una lista de las dimensiones que se pueden usar como entradas para generar consultas con la API de consulta.
- [Consulta](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): proporciona operaciones para obtener datos de costo y uso agregados en función de la consulta que proporcione. Mediante el uso de la API de consulta, puede especificar el filtrado, ordenación y agrupación que desee en todas las dimensiones disponibles (a las que se obtiene acceso desde la API de dimensiones).

**Costos pronosticados**

**¿Por qué no veo las previsiones de mis costos en el análisis de costos?**  
Hay varios motivos por los que puede faltar la proyección de pronósticos para usted en el análisis de costos, algunas de ellas son las siguientes:

1. Si los datos de costo tienen menos de 10 días de antigüedad, el gráfico de previsión no se cargará. El modelo necesita al menos 10 días de datos de costo reciente para proyecciones precisas.
2. Si ha seleccionado fechas históricas, el gráfico de previsión no estará visible. Seleccione un intervalo de fechas con fechas futuras para mostrar el gráfico de pronósticos.
3. Si la cuenta tiene varias monedas, el gráfico de previsión solo reducirá los costos de "todos los costos en USD"

**¿Por qué el pronóstico no cambia cuando se realizan cambios en los recursos?**  
El modelo de pronóstico requiere un par de días para tener en cuenta los cambios de la cuenta y no realiza proyecciones inmediatas en función de los cambios en los recursos.  
Para los pasos más grandes de incremento o disminución de recursos, el modelo tardará un poco más en ajustarse a estos cambios para tener en cuenta las anomalías

**¿Por qué el pronóstico aumenta después de realizar una reserva o comprar un Marketplace?**  
El modelo de previsión considera su "costo real" y no tiene en cuenta el uso y la compra por separado. Para una compra de pago único, el modelo reducirá las proyecciones después de 10 días para tener en cuenta el aumento repentino de los costos.

**Quiero ver las previsiones para una única dimensión (por ejemplo, Caudalímetro**  
La previsión actualmente es compatible con las proyecciones de costes totales y no con los medidores individuales. Por lo tanto, si se ' agrupa por ' una dimensión, las proyecciones serán para un total de todos los elementos de la dimensión.

**Documentos recomendados**

- [¿Qué es la administración de costos de Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedimientos recomendados de administración de costos de Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizar los gastos y los gastos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorar y analizar los costos con análisis de costos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Administración de costos de Azure: precios](https://azure.microsoft.com/services/cost-management/#pricing)
- [Revisión de costos en análisis de costos](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial en vídeo: crear un presupuesto en Azure portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Requisitos previos para ver y personalizar presupuestos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Creación y administración de presupuestos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurar la automatización con la API de presupuestos y grupos de acciones de Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Usar alertas de costos para supervisar el uso y los gastos](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedimientos recomendados de administración de costos](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vídeos de tutorial**

- [Crear un presupuesto en Azure portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Administrar costos con la API de presupuestos y grupos de acciones](https://go.microsoft.com/fwlink/?linkid=2147038)