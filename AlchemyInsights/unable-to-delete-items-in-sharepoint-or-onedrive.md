---
title: No se pueden eliminar elementos de SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038534"
---
# <a name="unable-to-delete-items"></a>No se pueden eliminar elementos

- Las directivas de retención pueden causar esto, debe deshabilitar o excluir la retención respectiva que está causando este problema. Después de quitar una directiva de retención o retención, el cambio puede tardar hasta 24 horas en tener efecto. Asegúrese de que no hay una configuración [de directiva de](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) retención en el elemento.

- Es posible que el sitio haya excedido el límite de almacenamiento, aumente la [cuota del sitio](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) y elimine el elemento.

- Asegúrese de que el elemento no [está desprote autenticado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para otro usuario.

- Por último, los administradores pueden usar SharePoint Patrones y [prácticas](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contiene una biblioteca de comandos de PowerShell que le permiten realizar acciones de administración complejas, como forzar la eliminación de elementos persistentes.
- [Quitar archivo PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Quitar carpeta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Quitar elemento de lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Quitar lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Quitar campo PNP (columna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)