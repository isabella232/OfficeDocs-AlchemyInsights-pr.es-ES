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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923661"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>¿Cuándo se sincronizan los cambios de mi perfil en la SharePoint de perfiles de usuario?

SharePoint Online usa el trabajo del temporizador De importación de Active Directory (AD Import) para importar usuarios y grupos a la aplicación de perfiles de usuario. 
  
1. AD Import sincroniza los cambios de la SharePoint de directorios en línea con la aplicación de perfil de usuario. Estos cambios se procesan en lotes.
    
2. El trabajo del temporizador se ejecuta hasta que se sincronizan los cambios.
    
> [!NOTE]
> El tiempo que tarda el trabajo en ejecutarse depende del número de cambios que se realicen. Un gran número de cambios tarda más tiempo. El Contrato de nivel de servicio (SLA) indica que un cambio en un usuario en el directorio SharePoint Online se reflejará en la aplicación de perfiles de usuario en 24 horas. 
  
[Más información sobre la sincronización de perfiles de usuario en SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

