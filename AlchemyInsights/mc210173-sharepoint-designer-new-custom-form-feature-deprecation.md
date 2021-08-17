---
title: 'MC210173: desuso de la nueva característica de formulario personalizado en SharePoint Designer'
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
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077697"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173: desuso de la nueva característica de formulario personalizado en SharePoint Designer

Hemos identificado un problema que afecta a la funcionalidad de SharePoint Designer para [crear formularios personalizados](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) en SharePoint Online. Después de un examen minucioso, hemos determinado que no hay ninguna corrección conocida para este problema y hemos optado por deshabilitar la característica de creación de formularios personalizados a partir del sábado 25 de abril de 2020, a las 3:00 AM UTC. Este cambio no afecta a la capacidad de editar formularios creados previamente u otras características existentes en SharePoint Online Designer.

Después de realizar este cambio, los usuarios pueden haber recibido el error: "No se pudieron guardar los cambios de la lista en el servidor" al crear nuevos formularios.

Los usuarios que hayan usado previamente SharePoint Designer para crear formularios personalizados pueden usar [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) para hacerlo.

PowerApps es una herramienta fácil y eficaz que permite a los usuarios que operan en la experiencia moderna de SharePoint Online crear y editar formularios personalizados para listas y bibliotecas de documentos de SharePoint directamente desde una ventana del explorador. PowerApps no necesita el conocimiento de codificación tradicional ni ninguna descarga adicional de la aplicación, como InfoPath.

**Nota**: los usuarios de la experiencia clásica de SharePoint Online tendrán que cambiar temporalmente a la experiencia moderna para tener acceso a PowerApps y poder usarlo. Sin embargo, todos los formularios personalizados creados en PowerApps son accesibles para los usuarios de la experiencia clásica de SharePoint Online.
