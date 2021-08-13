---
title: Restringir el acceso en SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093903"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir el acceso en SharePoint o OneDrive

Hay muchas maneras de restringir el acceso a SharePoint servicios online/OneDrive web. Estos distintos métodos de restricción de acceso se describen a continuación. 

**Restricción de permisos**

En SharePoint Online y OneDrive para la Empresa, se restringe el acceso a elementos como sitios, archivos y carpetas al conceder acceso únicamente a los grupos o personas que deben tener acceso.

- [Personalizar permisos para una SharePoint o biblioteca](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizar permisos del sitio de SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Cambiar permisos en una subcarpeta](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Control de acceso desde dispositivos no administrados](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como administrador SharePoint o global, puede bloquear o limitar el acceso a contenido de SharePoint y OneDrive desde dispositivos no administrados (aquellos que no son compatibles o unidos a AD híbridos en Intune).

**Restricción de ubicación de red**

Como administrador de TI, puede controlar el acceso a SharePoint y OneDrive en función de las ubicaciones de red definidas en las que confíe. Esto también se conoce como directiva basada en la ubicación. Para obtener más información, consulte [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restricción de bloqueo de sitio** 

En SharePoint Online tiene la capacidad de bloquear una colección de sitios, por lo que nadie tiene acceso. Esto se establece a través de PowerShell y [SharePoint Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) de administración en línea mediante la [propiedad Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir a los usuarios la creación de sitios o subsitios**

Como administrador SharePoint o administrador global, puede permitir que los usuarios creen y administren sus propios sitios de SharePoint, determinar qué tipo de sitios pueden crear y especificar la ubicación de los sitios. Para obtener más información, consulte [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

