---
title: No se puede agregar el flujo de trabajo de aprobación de 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020353"
---
# <a name="unable-to-add-2010-approval-workflow"></a>No se puede agregar el flujo de trabajo de aprobación de 2010

En una colección de sitios de Microsoft SharePoint, no puede agregar un flujo de trabajo reutilizable globalmente (como "Aprobación - SharePoint 2010") a una lista o biblioteca.
  
Para resolver este problema, siga estos pasos: 
  
1. Abra el sitio web raíz de la colección de sitios en SharePoint Designer 2013.
  
2. En **Objetos de sitio**, seleccione Flujos de **trabajo**. 
  
3. En la **sección Nuevo** de la cinta flujos **de trabajo,** seleccione **Flujo de trabajo reutilizable.** 
  
4. En el **formulario Crear flujo de trabajo** reutilizable, escriba el nombre ** *Repair2010* **. En **Tipo de plataforma,** haga clic SharePoint flujo de **trabajo de 2010** y, a continuación, haga clic en **Aceptar**. 
  
1. En la **sección Guardar** de la cinta de opciones **Flujo de** trabajo, seleccione **Publicar**. 
  
2. En la **sección Administrar** de la cinta de opciones **Flujo de** trabajo, seleccione **Publicar globalmente**. En el cuadro de diálogo de confirmación que aparece, seleccione **Aceptar**. 
  
3. En un explorador web, busque el sitio web raíz de la colección de sitios y, a continuación, acceda a **Site Configuración** Site \> **Collection Features**. Alterna la **característica Flujos de trabajo:** 
  
· Si la característica es  *Activada,*  haga clic **en Desactivar y, a continuación,** haga clic **en Activar**. 
  
· Si la característica está  *desactivada,*  haga clic **en Activar**. 
  
Para obtener más información, consulte el siguiente [artículo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

