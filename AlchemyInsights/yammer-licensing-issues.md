---
title: Problemas con la concesión de licencias de Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989752"
---
# <a name="yammer-licensing-issues"></a>Problemas con la concesión de licencias de Yammer

Todos los usuarios deben tener una licencia para usar el servicio de Yammer Enterprise, pero, de manera predeterminada, Yammer no necesita que los usuarios tengan una licencia para obtener acceso al servicio. Cuando un administrador cambia la configuración para bloquear a los usuarios de Microsoft 365 sin licencias de Yammer, los usuarios a los que no se les ha asignado una licencia de Yammer Enterprise no pueden obtener acceso al servicio de Yammer. Para obtener más información, vea [Administrar licencias de usuario de Yammer en Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365). 

Cuando se eliminan las licencias de los usuarios, ya no se muestra el icono de Yammer y otros servicios pueden usar la eliminación de la licencia para ocultar características. En otros casos, es posible que sigan apareciendo las características, pero que requieran una asignación de licencias para funcionar.  

**No se actualiza la licencia del usuario**  

En ocasiones, se asigna una licencia a un usuario, pero sigue sin poder tener acceso a Yammer. Es probable que se produzcan retrasos cuando se está realizando una asignación masiva de licencias. Es posible que los usuarios de Yammer no se actualicen en el mismo orden en que se cambiaron las licencias en Azure AD porque el sistema se ejecuta de forma asincrónica. Espere 24 horas antes de abrir un caso de soporte técnico para informar de problemas de sincronización de licencias.  

**Asignación masiva de licencias**  

Las licencias se pueden asignar mediante el centro de administración o mediante scripts de PowerShell. Para obtener más información, vea [Asignar licencias a los usuarios](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) y [Asignar licencias a cuentas de usuario con PowerShell de Office 365](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

El soporte técnico de Microsoft no proporciona asistencia para la creación de scripts, pero está disponible documentación sobre la asignación de licencias de Yammer. Para obtener más información, vea [Administración de licencias de Yammer mediante Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).