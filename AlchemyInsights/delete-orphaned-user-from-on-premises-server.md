---
title: Eliminar usuario huérfano del servidor local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102286"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Eliminar usuario huérfano del servidor local

Para quitar un usuario huérfano, siga estos pasos:

1. Fuerce la sincronización de directorios siguiendo las instrucciones en [¿Qué es la identidad híbrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Para comprobar la sincronización de directorios, consulte [¿Qué es la identidad híbrida con Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Si las funciones de sincronización son correctas pero la eliminación de objetos de Active Directory no se propaga a Azure AD, elimine manualmente el objeto huérfano mediante uno de los siguientes cmdlets del Módulo Azure Active Directory para Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Por ejemplo, para quitar el Id. de usuario huérfano iker.arteaga@contoso.com, creado originalmente con la sincronización de directorios, ejecute el cmdlet:

    Remove-MsolUser –UserPrincipalName Iker.Arteaga@Contoso.com