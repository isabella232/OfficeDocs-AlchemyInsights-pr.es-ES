---
title: No se puede agregar una cuenta después de actualizar a macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475131"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>No se puede agregar una cuenta después de actualizar a macOS 11.6 Big Sur

Después de actualizar a macOS 11.6, es posible que su cuenta OneDrive profesional o educativa o su cuenta personal de OneDrive no aparezca en la lista de cuentas y es posible que no pueda iniciar sesión en una segunda cuenta desde la aplicación.

Se ha desarrollado una corrección para este problema. En primer lugar, determine si está ejecutando la versión independiente o de la Tienda de aplicaciones de OneDrive:

- Seleccione la nube en OneDrive en la barra de menús > **Ayuda & Configuración** > **Preferencias** > **Acerca de**. Si el número de versión no incluye **(Independiente),** tiene la versión de la tienda de aplicaciones del producto.

Si usa la versión independiente de OneDrive, reinicie el equipo y las actualizaciones automáticas de OneDrive para realizar una compilación donde se resuelva este problema. Si quiere instalar la compilación manualmente, descargue este [archivo .zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), descomprima el archivo y copie la aplicación OneDrive en la carpeta Aplicaciones (reemplazando la aplicación OneDrive existente).

Si está usando la versión de la tienda de aplicaciones, considere la posibilidad de instalar la versión independiente de OneDrive. Esta versión funciona de la misma manera que la versión de la tienda de aplicaciones, pero permite a Microsoft ofrecer actualizaciones más rápidamente a los usuarios y las conecta a una versión que incluye la corrección de este problema.

1. Descargue la versión independiente de [OneDrive que incluye la corrección](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Descomprima el archivo y copie la aplicación OneDrive en la carpeta Aplicaciones (reemplazando la aplicación OneDrive existente).

Si necesita usar la versión de la tienda de aplicaciones, espere a que la tienda de aplicaciones libere una versión de la aplicación que incluya la corrección. Desafortunadamente, Microsoft no puede comunicar una fecha estimada para que una versión no editable se libere de la tienda de aplicaciones.


