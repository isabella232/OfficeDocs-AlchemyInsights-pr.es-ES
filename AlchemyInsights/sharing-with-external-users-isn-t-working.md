---
title: El uso compartido con usuarios externos no funciona
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304386"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Corregir problemas para compartir SharePoint contenido con usuarios externos

Asegúrese de que el uso compartido externo está activado para su organización:
  
1. Vaya a la página Complementos de servicios en el [ &amp; Centro de administración de Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)y haga clic en **Sitios**.
    
2. Asegúrese de que la configuración esté activada. Si está seleccionado "Solo los usuarios externos existentes", asegúrese de que el usuario externo aparece en el Centro de administración de Microsoft 365.
    
Asegúrese de que el uso compartido externo esté activado para el sitio. Para una colección de sitios clásica:
  
1. En el nuevo centro SharePoint administración, en el panel izquierdo, haga clic en **sitios**.
    
2. Seleccione el sitio o los sitios y, en la cinta de opciones, haga clic en **Compartir**.
    
Para un sitio de grupo que pertenece a un grupo Microsoft 365 o a un sitio de comunicación:
  
- Estos nuevos tipos de sitio tienen la misma configuración de uso compartido que la configuración de toda la organización, a menos que la configuración de toda la organización permita compartir archivos mediante vínculos que no requieren inicio de sesión. En este caso, los sitios permiten compartir con usuarios externos nuevos y existentes que inician sesión. Para cambiar la configuración de sitios específicos, use el nuevo centro SharePoint administración o PowerShell. [Más información](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Nota:** La configuración de uso compartido externo para cualquier sitio puede ser más restrictiva que la configuración de toda la organización, pero no más permisiva que la configuración de toda la organización. 
  

