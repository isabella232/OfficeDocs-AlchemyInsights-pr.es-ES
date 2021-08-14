---
title: OneDrive para la Empresa Web OneDrive redirige a Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923004"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirigido a Delve después de hacer clic en OneDrive

Consulte nuestra guía de [solución de problemas detallada.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Para resolver este problema, el administrador debe conceder a los usuarios el derecho de crear su sitio de Mis sitios. Esto se debe a que la OneDrive para la Empresa se crea en Mis sitios.

Para conceder este derecho, siga estos pasos:

1. En el Centro SharePoint administración, haga clic en **Perfiles de usuario**.

2. En la **sección Personas,** haga clic **en Administrar permisos de usuario**.

3. Agregue usuarios que necesiten permisos para crear su sitio de Mis sitios. De forma predeterminada, esta configuración se establece en **Todos excepto los usuarios externos.**

4. Después de agregar el usuario, los usuarios o el grupo, asegúrese de que el usuario, los usuarios o el grupo agregados están **seleccionados,** desplácese a la sección de permisos y, a continuación, active la casilla junto a Crear sitio **personal (necesario** para el almacenamiento personal, el servicio de noticias y el contenido seguido).

5. Haga **clic en** Aceptar y, a continuación, haga que el usuario vaya a la OneDrive para crear el sitio.
