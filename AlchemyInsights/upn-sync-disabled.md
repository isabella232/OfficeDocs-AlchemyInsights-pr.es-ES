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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038129"
---
# <a name="upn-sync-disabled"></a>Sincronización upn deshabilitada

Si empezó a sincronizar con Azure AD antes del 30 de marzo de 2016, ejecute el siguiente cmdlet de PowerShell de Azure AD para habilitar solo la coincidencia de UPN para su organización:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
La coincidencia suave de UPN se activa automáticamente para las organizaciones que empezaron a sincronizarse con Azure AD en o después del 30 de marzo de 2016.
  
Para obtener más información sobre cómo habilitar la coincidencia suave en UPN y otras características de sincronización, consulte [Azure AD Conectar sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

