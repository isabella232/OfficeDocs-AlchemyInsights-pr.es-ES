---
title: Dispositivos no Windows de Protección contra amenazas avanzada (ATP) de Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967818"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Dispositivos no Windows de Protección contra amenazas avanzada (ATP) de Microsoft Defender

A continuación se muestra cómo hacerlo:

1. Siga la documentación de terceros para desconectar la solución de terceros de ATP de Microsoft Defender.
2. Desde el Azure Active Directory inquilino, quite los permisos de la solución de terceros:

    1. Inicie sesión en el [portal de Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Seleccione **Todos los servicios**  >  **Azure Active Directory** Enterprise  >  **aplicaciones**.
    1. Selecciona la aplicación que quieras quitar.
    1. Seleccione **Eliminar**.

Para obtener más información, [vea Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).
