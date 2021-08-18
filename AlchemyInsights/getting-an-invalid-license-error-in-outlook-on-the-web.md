---
title: 125 Obtener un error de licencia no válido en Outlook en la Web?
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 357e57d20e3b6f56d3058bc1c782c3da7598520c29c5c29bfba6eec614fc5248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54089277"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a>Obtener un error de licencia no válido en Outlook en la Web?

Si está usando Outlook en la Web y obtiene un error **De** algo salió mal que contiene **X-OWA-Error: Microsoft.Exchange. Datos. Storage. InvalidLicenseException**, la Exchange Online licencia no está asignada correctamente o ha expirado recientemente. El administrador puede asignarle una licencia siguiendo estos pasos:
  
1. Abra el [Centro de administración de Microsoft 365](https://portal.office.com/adminportal/home#/homepage) y, en **Usuarios activos,** seleccione **Editar un usuario**.

2. En la **página Editar un usuario** que se abre, seleccione el usuario. En la página de propiedades de usuario que se abre, haga clic **en Editar** para licencias **de producto.**

3. En la **página Licencias de productos** que se abre, seleccione el valor **location** adecuado y asigne una licencia que contenga Exchange Online (expanda la licencia para ver sus detalles). Cuando haya terminado, haga clic en **Guardar**.
