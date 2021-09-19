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
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446747"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>No se puede agregar una cuenta después de actualizar a macOS 11.6 Big Sur

Después de actualizar a macOS 11.6, es posible que su cuenta OneDrive profesional o educativa o su cuenta personal de OneDrive no aparezca en la lista de cuentas y es posible que no pueda iniciar sesión en una segunda cuenta desde la aplicación.

Se trata de un problema emergente relacionado con la actualización de macOS 11.6. Hasta que se resuelva el problema, puede acceder a su contenido de OneDrive desde la web o desde su dispositivo móvil. Microsoft está trabajando con Apple para restaurar la funcionalidad de OneDrive.

También puede iniciar la instancia de OneDrive que falta manualmente mediante Terminal. 

**Nota**: Esta solución alternativa solo funciona hasta que se reinicie OneDrive (ya sea mediante un reinicio de la máquina o una actualización de la aplicación de OneDrive).

Si la instancia que falta es la cuenta personal, abra Terminal y escriba:

`open "/Applications/OneDrive.app" --new --args /client=Personal`

Si la instancia que falta es la cuenta profesional o educativa, abra Terminal y escriba:

`open "/Applications/OneDrive.app" --new --args /client=Business1`

