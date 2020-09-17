---
title: Cómo habilitar el SSO sin problemas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780544"
---
# <a name="how-to-enable-seamless-sso"></a>Cómo habilitar el SSO sin problemas

Habilite SSO sin problemas a través de [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Si va a realizar una instalación nueva de Azure AD Connect, elija la [ruta de instalación personalizada](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). En la página **Inicio de sesión de usuario** , seleccione la opción Habilitar el inicio de **sesión único** .
  
Para comprobar que ha habilitado el SSO sin problemas correctamente:
  
1. Inicie sesión en el [centro de administración de Azure Active Directory](https://aad.portal.azure.com) como administrador global.

2. Seleccione **Azure Active Directory** en el panel izquierdo.

3. Compruebe que el inicio de sesión único sin problemas está **habilitado**.

Para obtener más información, vea [Inicio de sesión único de inicio sencillo de Azure Active Directory: Inicio rápido](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  