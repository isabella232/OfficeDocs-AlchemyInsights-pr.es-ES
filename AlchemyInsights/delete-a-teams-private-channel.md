---
title: Eliminar un canal privado de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730932"
---
# <a name="delete-a-teams-private-channel"></a>Eliminar un canal privado de Teams

Microsoft es consciente de un problema al eliminar un canal privado de Teams si tiene habilitadas las directivas de retención de SharePoint para el sitio de SharePoint subyacente. Microsoft está trabajando para solucionar este problema. Mientras tanto, puede usar una de las siguientes soluciones alternativas para eliminar dicho canal privado.

**Excluya la colección equipo/sitio de la directiva de retención de SharePoint.**

1. Diríjase al portal de administración de Office 365 y seleccione **Mostrar todo** en el panel de navegación izquierdo.
2. En **Centros de administración**, diríjase a **Seguridad y cumplimiento** > **Prevención de pérdida de datos** > **Directiva**.
3. Identifique cualquier directiva que se aplique a los sitios de SharePoint y modifíquela, de manera que el sitio de SharePoint para el equipo que contiene el canal privado NO se incluya en la directiva de retención.
4. Guarde la directiva.
    Las configuraciones de directivas pueden tardar hasta 24 horas en tener efecto.
    Después de que se haya excluido el sitio, puede eliminar el canal privado.  
    
Es ***posible*** que pueda eliminar el canal privado desde Microsoft Teams en su dispositivo Android. 

Para obtener información relacionada con SharePoint, consulte [No se pueden eliminar elementos en SharePoint Online o OneDrive para la Empresa](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).