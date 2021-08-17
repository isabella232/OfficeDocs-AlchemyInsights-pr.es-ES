---
title: Guardar sitio o lista como plantilla
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109221"
---
# <a name="save-site-or-list-as-a-template"></a>Guardar sitio o lista como plantilla

Las plantillas de sitio de SharePoint son definiciones preintegradas diseñadas en torno a una necesidad empresarial concreta. Para obtener más información, vea [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Estos son algunos problemas o soluciones comunes relacionados con guardar un sitio o una lista como plantilla en SharePoint Online.

**El botón Guardar plantilla de sitio o lista no está disponible o falta**. 

- Los administradores deben permitir el script personalizado para poder habilitar las características de la plantilla. Para obtener pasos detallados, ejemplos y consideraciones, [vea Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- El comando de Guardar sitio como plantilla no es compatible y puede causar problemas en los sitios que usen la infraestructura del servidor de publicación de SharePoint.


**La plantilla de sitio no se puede crear o no funciona correctamente**

- Es posible que falte una [característica](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a la plantilla y no se active. Si la característica no está disponible para activarla en la colección de sitios actual, no podrá usar la plantilla de sitio para crear un sitio.


- Compruebe si alguna de las listas o bibliotecas supera [el límite de umbral de vista de lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 elementos, ya que esto puede bloquear la creación de una plantilla de sitio.


- El sitio puede estar usando demasiados recursos y, por lo tanto, la plantilla de sitio supera el límite de 50 megabytes (MB).


- Hay problemas para mostrar los datos de una lista que utiliza una columna de búsqueda. Para obtener más información, vea Lista generada por plantillas no muestra datos de la lista de búsqueda [correcta en SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Para obtener información más detallada sobre problemas y soluciones comunes, consulte [Crear y usar plantillas de sitio.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

