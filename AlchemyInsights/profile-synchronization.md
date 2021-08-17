---
title: Sincronización de perfiles
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320726"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>¿Cuándo se sincronizan los cambios de mi perfil en la SharePoint de perfiles de usuario?

SharePoint Online usa el trabajo del temporizador De importación de Active Directory (AD Import) para importar usuarios y grupos a la aplicación de perfiles de usuario. 
  
1. AD Import sincroniza los cambios de la SharePoint de directorios en línea con la aplicación de perfil de usuario. Estos cambios se procesan en lotes.
    
2. El trabajo del temporizador se ejecuta hasta que se sincronizan los cambios.
    
**Nota:** El tiempo que tarda el trabajo en ejecutarse depende del número de cambios que se realicen. Un gran número de cambios tarda más tiempo. El Contrato de nivel de servicio (SLA) indica que un cambio en un usuario en el directorio SharePoint Online se reflejará en la aplicación de perfiles de usuario en 24 horas. 
  
[Más información sobre la sincronización de perfiles de usuario en SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

