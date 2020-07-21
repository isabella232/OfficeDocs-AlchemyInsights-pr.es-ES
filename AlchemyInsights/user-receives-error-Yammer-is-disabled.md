---
title: El usuario recibe el error AADSTS7000112 Yammer is disabled
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157335"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>El usuario recibe el error AADSTS7000112 Yammer is disabled

Si recibe el error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", hay un problema con la entidad de servicio en Azure AD. Es posible que el administrador haya deshabilitado la entidad de servicio para bloquear el acceso a Yammer.

No se recomienda deshabilitar la entidad de servicio, porque puede provocar problemas adicionales. Para obtener más información sobre el método admitido para bloquear el acceso de los usuarios a Yammer, vea [Desactivar el acceso de usuarios de Microsoft 365 a Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Para corregir este problema en Azure Portal y restaurar el acceso de los usuarios a Yammer, haga lo siguiente:

1.  Abra la página de Azure Active Directory y seleccione **Aplicaciones empresariales** en **Administrar** en el panel de navegación izquierdo.
3.  Escriba **Yammer de Office 365** en el cuadro de búsqueda y seleccione el nombre de la aplicación para abrir configuración.
4.  Seleccione **Propiedades** en **Administrar** en el panel de navegación izquierdo.
5.  Establezca el valor **¿Habilitado para que los usuarios inicien sesión?** en **Sí** y, después, seleccione **Guardar**.
6.  Vuelva a iniciar sesión en Yammer. Es posible que deba borrar las cookies.

También puede ejecutar los comandos de PowerShell para establecer el valor. Para obtener más información, vea ["Lo sentimos, pero estamos teniendo problemas para iniciar su sesión" al hacer clic en el icono de Yammer en Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 