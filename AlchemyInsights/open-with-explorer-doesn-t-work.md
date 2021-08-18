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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321878"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir con el Explorador no funciona

Si **Abrir con el Explorador** o **Ver** en el Explorador de archivos no funciona, asegúrese de que el servicio WebClient esté establecido en **Ejecutar** siguiendo los pasos siguientes. Por ejemplo, puede tardar mucho tiempo en abrir una biblioteca SharePoint o OneDrive cuando el servicio no se está ejecutando. 
  
1. En el Windows de búsqueda, escriba **ejecutar,** seleccione ejecutar aplicación de escritorio, escriba services.msc y, a continuación, seleccione Entrar .
    
2. Desplácese hacia abajo hasta el servicio WebClient y compruebe la **columna** Estado. Si el estado del servicio WebClient no se está **ejecutando,** haga doble clic en el servicio, haga clic en **Inicio** y, a continuación, haga clic en **Aceptar**. Habilite el servicio, si es necesario, seleccionando **Manual** o **Automático** en el cuadro **Tipo de** inicio. 
    
**Nota:** Para solucionar problemas que se abren en el Explorador de archivos, vea [Abrir en el Explorador](https://go.microsoft.com/fwlink/?linkid=871665). Explorar la sincronización como una mejor alternativa: [sincronizar SharePoint archivos con el nuevo Sincronización de OneDrive cliente](https://go.microsoft.com/fwlink/?linkid=871666). 
  

