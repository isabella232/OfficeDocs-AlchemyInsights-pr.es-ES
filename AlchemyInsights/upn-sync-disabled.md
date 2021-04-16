---
title: Sincronización upn deshabilitada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782168"
---
# <a name="upn-sync-disabled"></a>Sincronización upn deshabilitada

Si empezó a sincronizar con Azure AD antes del 30 de marzo de 2016, ejecute el siguiente cmdlet de PowerShell de Azure AD para habilitar solo la coincidencia de UPN para su organización:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
La coincidencia suave de UPN se activa automáticamente para las organizaciones que empezaron a sincronizarse con Azure AD en o después del 30 de marzo de 2016.
  
Para obtener más información sobre cómo habilitar la coincidencia suave en UPN y otras características de sincronización, consulte Características del servicio de sincronización de [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

