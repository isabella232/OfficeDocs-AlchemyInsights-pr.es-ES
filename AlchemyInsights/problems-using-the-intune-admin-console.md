---
title: Problemas con el uso de la consola de administración de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728304"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemas con el uso de la consola de administración de Intune

**"Acceso denegado" al navegar por el portal de administración de Intune.**

- Si es miembro de un rol personalizado de Intune, asegúrese de que se ha asignado una licencia de Intune o de Enterprise Mobility Suite (EMS) a su cuenta.
- Si usa Configuration Manager para administrar dispositivos, compruebe que usted no forma parte del conjunto de usuarios de Intune para la MDM de Configuration Manager.
- Compruebe que se le han asignado los permisos adecuados de control de administración basado en roles (RBAC) en la hoja de roles de Intune.
- Compruebe que el grupo usado no es una lista de distribución. Intune en el Microsoft Azure Portal solo admite cuentas de usuario que pertenecen a grupos de seguridad de Azure Active Directory. Revisar los grupos en el portal de Azure > **Intune** > **Grupos**, o en Microsoft Azure Portal > **Azure Active Directory**.

**El usuario tiene demasiados permisos para la función Intune asignada**

Aconseje al usuario que vaya a **Intune** > **Roles de Intune** > **Mis permisos** > **Exportar** para revisar los permisos concedidos.

**He agregado un grupo de ámbito a un rol, pero los usuarios de ese rol aún ven a otros usuarios o dispositivos.**

Los grupos de ámbito no filtran usuarios o dispositivos. Grupos de ámbito:

- Limitar qué usuarios pueden asignar directivas o aplicaciones.
- Permitir que solo usuarios específicos ejecuten tareas remotas en dispositivos.

Para obtener más información sobre los grupos de ámbito, consulte [Control de acceso basado en roles (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Agregué un usuario a un rol de Intune, pero aún tienen acceso total a la consola de administración de Intune.**

Desplácese hasta Intune > **Usuarios** en el Microsoft Azure Portal y compruebe que el usuario no tiene asignado ninguno de los siguientes roles en el portal de Azure:

- Administrador global
- Administrador de servicios de Intune
- Administrador de SharePoint

Para más información, consulte [Control de acceso basado en roles (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemas de acceso**

Para más información, consulte [No puedo iniciar sesión en Office 365, Azure o Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).