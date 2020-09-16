---
title: Sincronización UPN deshabilitada
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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749531"
---
# <a name="upn-sync-disabled"></a>Sincronización UPN deshabilitada

Si empezó a sincronizar con Azure AD antes del 30 de marzo de 2016, ejecute el siguiente cmdlet de Azure AD PowerShell para habilitar la coincidencia simplificada de UPN para su organización solo:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $True**
  
La coincidencia Soft de UPN se activa automáticamente para las organizaciones que comenzaron a sincronizarse con Azure AD a partir del 30 de marzo de 2016.
  
Para obtener más información acerca de cómo habilitar la coincidencia flexible en UPN y otras características de sincronización, consulte [características del servicio de sincronización de Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

