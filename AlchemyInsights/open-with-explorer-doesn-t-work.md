---
title: Abrir con el Explorador no funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011353"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir con el Explorador no funciona

Si **Abrir con el Explorador** o **Ver** en el Explorador de archivos no funciona, asegúrese de que el servicio WebClient esté establecido en **Ejecutar** siguiendo los pasos siguientes. Por ejemplo, puede tardar mucho tiempo en abrir una biblioteca SharePoint o OneDrive cuando el servicio no se está ejecutando. 
  
1. En el Windows de búsqueda, escriba **ejecutar,** seleccione ejecutar aplicación de escritorio, escriba services.msc y, a continuación, seleccione Entrar .
    
2. Desplácese hacia abajo hasta el servicio WebClient y compruebe la **columna** Estado. Si el estado del servicio WebClient no se está **ejecutando,** haga doble clic en el servicio, haga clic en **Inicio** y, a continuación, haga clic en **Aceptar**. Habilite el servicio, si es necesario, seleccionando **Manual** o **Automático** en el cuadro **Tipo de** inicio. 
    
> [!NOTE]
> Para solucionar problemas de apertura en el Explorador de archivos, vea [Abrir en el Explorador](https://go.microsoft.com/fwlink/?linkid=871665). Explorar la sincronización como una mejor alternativa: [sincronizar SharePoint archivos con el nuevo Sincronización de OneDrive cliente](https://go.microsoft.com/fwlink/?linkid=871666). 
  

