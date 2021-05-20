---
title: Crear usuario
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569764"
---
# <a name="create-user"></a>Crear usuario

**ANUNCIO:**

- Desuso de la compatibilidad de inicio de sesión de WebView desde Google a partir del [4 de enero de 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Compruebe si las aplicaciones pueden verse afectadas por seguir las instrucciones [de Google](https://go.microsoft.com/fwlink/?linkid=2157323) sobre la compatibilidad de pruebas.
- Asegúrate de usar la vista web del sistema o el explorador del sistema al iniciar sesión en los usuarios con cuentas de Google de consumidor. Para más información, consulte [Cómo iniciar sesión en las aplicaciones solo con el explorador Chrome](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**No puedo crear un usuario en mi directorio de Azure AD**

1. Asegúrese de que está autorizado para crear un nuevo usuario estándar. Solo el rol Administrador global o Administrador de usuarios en Azure Active Directory (AD) puede crear un nuevo usuario estándar. Si no tiene uno de estos roles, pida a un administrador que le agregue a uno de estos roles o que cree la nueva cuenta de usuario.
1. Asegúrese de que el nombre de usuario está en un dominio comprobado en su Azure AD. Si no tiene nombres de dominio personalizados comprobados en su Azure AD, puede usar su dominio inicial de Azure AD, que termina con *.onmicrosoft.com.
1. Asegúrese de que el nombre de usuario está en un dominio que no está federado con Azure AD desde su AD local. Los usuarios no se pueden agregar a la nube con nombres de dominio federados desde la implementación local.
1. Asegúrese de que ningún otro usuario o contacto ya tenga el nombre de usuario que desea asignar al nuevo usuario. Los nombres de usuario deben ser únicos en Azure AD.
1. Consulte [Roles y administradores de Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para su Azure AD.
1. Consulte los [nombres de dominio](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para su Azure AD.
1. Revise los [Registros de auditoría](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para ver información más detallada sobre un usuario creado o eliminado recientemente, como quién realizó la acción y cuándo.
1. Para obtener más información sobre cómo agregar nuevos usuarios, vea [Usar Azure Portal para crear un nuevo usuario en Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Roles administrativos de Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)permisos de rol de administrador en Azure Active Directory
1. También puede usar [PowerShell de Azure AD para crear un nuevo usuario.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
