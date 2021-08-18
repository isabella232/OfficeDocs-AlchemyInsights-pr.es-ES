---
title: Solucionar problemas con Open with Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323583"
---
# <a name="fix-problems-with-open-with-explorer"></a>Corregir problemas con Abrir con el Explorador

Se solucionan problemas comunes al abrir una biblioteca de documentos SharePoint o OneDrive mediante el **comando Abrir con explorador:** 
  
- Use Internet Explorer 10 o Internet Explorer 11. **Abrir con explorer** no es compatible con Microsoft Edge, Google Chrome, Firefox y otros. **Abrir con el Explorador** está deshabilitado en todos los exploradores excepto Internet Explorer. 
    
- **Abrir con el Explorador** no está disponible en la experiencia moderna para SharePoint bibliotecas. En **su lugar, use Vista en el Explorador de** archivos. Seleccione **Ver opciones** Ver en el Explorador de \> **archivos**. La vista en el Explorador de archivos no es compatible con Microsoft Edge, Google Chrome, Firefox y otros. **Vista en el Explorador de** archivos en disponible solo en Internet Explorer. 
    
- Asegúrese de que el servicio WebClient se está ejecutando. En el Windows de búsqueda, escriba ejecutar, seleccione ejecutar aplicación de escritorio, escriba services.msc y, a continuación, presione ENTRAR. Desplácese hacia abajo hasta el servicio WebClient y asegúrese de que la **columna Estado** muestra "En ejecución". Si no lo hace, haga doble clic en el servicio, haga clic en **Inicio** y, a continuación, haga clic en **Aceptar**. (Es posible que deba habilitar primero el servicio seleccionando **Manual** o **Automático** en el cuadro **Tipo de** inicio). 
    
**Nota:** Abrir una biblioteca en el Explorador de archivos es útil si necesita copiar o mover varios archivos y carpetas una vez, pero si desea trabajar regularmente en la biblioteca, se recomienda sincronizarla. Para solucionar problemas de apertura en el Explorador de archivos, vea [Abrir en el Explorador](https://go.microsoft.com/fwlink/?linkid=871665). Para obtener información sobre cómo configurar la sincronización, [consulta Sincronizar SharePoint archivos con el nuevo Sincronización de OneDrive cliente](https://go.microsoft.com/fwlink/?linkid=871666).
  
Vea el artículo Cómo usar el [comando "Abrir](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) con explorador" para solucionar problemas en SharePoint Online para obtener más información. 
  

