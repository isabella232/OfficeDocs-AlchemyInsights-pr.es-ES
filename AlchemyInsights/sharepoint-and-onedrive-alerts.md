---
title: Retrasos en la recepción de alertas de SharePoint y OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727260"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Retrasos en la recepción de alertas de SharePoint y OneDrive

- Compruebe primero la carpeta de correo no deseado o no deseado en el correo electrónico.
- Si **se retrasan todas las alertas de varios archivos o bibliotecas**, visite el [Panel de estado del servicio](https://portal.office.com/adminportal/home?ref=/servicehealth) para comprobar si hay algún asesor o incidente que pueda estar ocurriendo con SharePoint o Exchange. El problema puede deberse a la capacidad de alerta de SharePoint o a los retrasos en los correos electrónicos a través de Exchange. Además, tenga en cuenta si se está entregando otro correo electrónico (si no es así, es probable que el problema se produzca con retrasos de Exchange).
- Si **no se entrega una alerta individual de un archivo o biblioteca específicos**, intente eliminarla y volver a crearla. Consulte [administrar, ver o eliminar alertas de SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para volver a crear la alerta.

> [!NOTE]
> - No se pueden enviar alertas a un grupo de distribución. Solo se admiten los grupos de seguridad y de O365.
> - No puede personalizar las plantillas de correo electrónico de alerta. Debe usar el flujo de trabajo de Microsoft Flow o SharePoint Designer para conseguirlos.
