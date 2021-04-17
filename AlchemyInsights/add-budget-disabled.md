---
title: ¿Por qué el botón Agregar presupuesto está deshabilitado para mí?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822652"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>¿Por qué el botón Agregar presupuesto está deshabilitado para mí?

Para crear un presupuesto, necesita uno de los siguientes permisos:

- Grupo de administración, Suscripción, Ámbitos de grupo de recursos
- Colaborador de administración de costos
- Owner
- Colaborador
- Solo cliente de empresa: inscripción, departamento, ámbitos de cuenta
- Administrador de inscripción (establecer presupuesto en el ámbito de inscripción)
- Administrador del departamento (establecer el presupuesto en el ámbito del departamento)
- Propietario de la cuenta (establecer presupuesto en el ámbito cuenta)
- Solo contrato de cliente moderno: cuenta de facturación, perfil de facturación, ámbitos de sección factura
- Creador de suscripciones de Azure

**Creé un presupuesto cuando el costo del mes actual ya estaba sobre presupuestado. ¿Por qué no he recibido una alerta?**  
Si ya ha superado un umbral de costo determinado al crear un presupuesto, esa alerta no se disparará. Una vez que se inicia un nuevo ciclo, si se rompe el umbral, se disparará la alerta.

**¿Cuándo debo esperar recibir una alerta después de superar uno de mis umbrales de alerta presupuestados definidos?**  
Los presupuestos se evalúan cada 4 horas. Los datos de uso tardan como mínimo 8 horas en llegar al sistema de presupuestos. Dado esto, las alertas pueden tardar hasta 12 horas en dispararse después de superar un umbral.

**¿Por qué se deshabilita el botón Fecha de inicio cuando selecciono un período de restablecimiento de mes o mes de facturación?**  
Los presupuestos se alinean con el mes calendario actual o el período de facturación actual (en el caso de que se seleccione Mes de facturación). Por lo tanto, rellenamos previamente este valor por usted.

**¿Por qué no veo un gráfico de mis costos en la experiencia de creación de presupuesto?**  
Necesitamos un mínimo de 2 meses de datos de costos antes de poder representar un gráfico para ayudarle con la creación de presupuesto.

**¿Por qué no puedo establecer un presupuesto en una suscripción que acabo de crear?**  
Después de la creación de una suscripción, los datos tardan entre 24 y 48 horas en procesarse antes de establecer un presupuesto en ella.

**Recursos de api de presupuesto**

- [API de presupuestos v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)proporciona operaciones para crear y actualizar presupuestos. Con la API de Presupuestos, puede establecer un umbral presupuestado y configurar varias alertas para que se desprendan a medida que se acerca a ese umbral. Las alertas pueden desencadenar un correo electrónico o un grupo de acciones de Azure para realizar la automatización. Nota: El filtrado de esta API no se alinea con las dimensiones ni el filtrado de la API de consulta.
- [API de presupuestos v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)crear presupuestos con mayores capacidades de filtrado de costos que v1. El filtrado se alinea con el contrato usado en nuestras API de consulta y dimensiones. Esta es la API de presupuestos recomendada para usar en adelante.
- [Dimensiones:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)proporciona operaciones para obtener dimensiones admitidas para su uso en una variedad de ámbitos. Con la API de dimensiones, puede recuperar una lista de dimensiones que se pueden usar como entradas para generar consultas con la API de consulta.
- [Consulta:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)proporciona operaciones para obtener datos agregados de costo y uso en función de la consulta que proporcione. Con la API de consulta, puede especificar el filtrado, ordenación y agrupación deseados en todas las dimensiones disponibles (a las que se accede desde la API de dimensiones).

**Costos previstos**

**¿Por qué no veo previsiones de mis costos en análisis de costos?**  
Hay varias razones por las que la proyección de previsión podría faltar en el análisis de costos, algunas de ellas son las siguientes:

1. Si los datos de costo tienen menos de 10 días de antigüedad, el gráfico de previsiones no se cargará. El modelo requiere al menos 10 días de datos de costos recientes para proyecciones precisas
2. Si ha seleccionado fechas históricas, el gráfico de previsiones no estará visible. Seleccione un intervalo de fechas con fechas futuras para que se muestre el gráfico de previsiones
3. Si su cuenta tiene varias monedas, el gráfico de previsiones solo proyectará los costos de "Todos los costos en USD"

**¿Por qué no cambia la previsión al realizar cambios en mis recursos?**  
El modelo de previsión requiere un par de días para tener en cuenta los cambios en la cuenta y no realiza proyecciones inmediatas en función del cambio en los recursos  
Para mayores pasos de aumento o disminución de recursos, el modelo tarda un poco más en ajustarse a estos cambios para tener en cuenta las anomalías

**¿Por qué aumenta mi previsión después de realizar una reserva o una compra de Marketplace?**  
El modelo de previsión tiene en cuenta el "costo real" y no tiene en cuenta el uso y la compra por separado. Para una compra única, el modelo disminuirá las proyecciones después de 10 días para tener en cuenta el aumento repentino de los costos

**Quiero ver previsiones para una sola dimensión (por ejemplo. Meter)**  
Actualmente, forecast admite proyecciones de costo total y no para contadores individuales. Por lo tanto, cuando "Agrupado por" una dimensión, las proyecciones serán para el total de todos los elementos de la dimensión

**Documentos recomendados**

- [¿Qué es Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedimientos recomendados de Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizar sus costos y gastos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorar y analizar costos con el análisis de costos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Administración de costos de Azure: precios](https://azure.microsoft.com/services/cost-management/#pricing)
- [Revisar los costos en el análisis de costos](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial en vídeo: Crear un presupuesto en Azure Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Requisitos previos para ver y personalizar presupuestos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Crear y administrar presupuestos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurar la automatización con la API de Grupos de acciones de Azure y Presupuestos](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Usar alertas de costos para supervisar el uso y el gasto](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Procedimientos recomendados de administración de costos](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vídeos tutoriales**

- [Crear un presupuesto en Azure Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Administrar costos con la API de Presupuestos y grupos de acciones](https://go.microsoft.com/fwlink/?linkid=2147038)