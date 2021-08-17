---
title: Crear un sitio en SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057983"
---
# <a name="create-sharepoint-sites-using-templates"></a>Crear SharePoint con plantillas

La capacidad para guardar un sitio como plantilla no es compatible con los sitios modernos de Comunicación o de Equipo. Para obtener más información sobre el uso de plantillas, consulte [Guardar, descargar y cargar un sitio de SharePoint como plantilla](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Estos son algunos problemas o soluciones comunes relacionados con guardar un sitio o una lista como plantilla en Sharepoint Online. 

**El botón Guardar plantilla de sitio/lista no está disponible o falta**

Los administradores deben permitir el script personalizado para poder habilitar las características de la plantilla. Para obtener pasos detallados, ejemplos y consideraciones, vea 

- [Permitir o impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- El comando de Guardar sitio como plantilla no es compatible y puede causar problemas en los sitios que usen la infraestructura del servidor de publicación de SharePoint.

**La plantilla de sitio no se puede crear o no funciona correctamente**

Es posible que falte una [característica](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a la plantilla y no se active. Si la característica no está disponible para activarla en la colección de sitios actual, no podrá usar la plantilla de sitio para crear un sitio.

- Compruebe si alguna de las listas o bibliotecas supera [el límite de umbral de vista de lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 elementos, ya que esto puede bloquear la creación de una plantilla de sitio.

- Es posible que el sitio use demasiados recursos y, por lo tanto, la plantilla de sitio supere el límite de 50 MB.


- Hay problemas para mostrar los datos de una lista que utiliza una columna de búsqueda. Para obtener más información, consulte [La lista generada por plantilla no muestra los datos correctos para una columna en SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Para obtener información más detallada sobre problemas y soluciones comunes, consulte [Crear y usar plantillas de sitio.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



