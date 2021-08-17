---
title: Ayuda con la configuración de la pantalla de luz nocturna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078747"
---
# <a name="help-with-the-night-light-display-setting"></a>Ayuda con la configuración de la pantalla de luz nocturna

Para obtener más información sobre la configuración de la pantalla de luz nocturna, vea [Configurar la pantalla de luz nocturna en Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Si las opciones de luz nocturna están atenuadas en Configuración, compruebe la pantalla: 

1. Haga clic en el cuadro de búsqueda de la barra de tareas y escriba **Administrador de dispositivos** y, después, seleccione **Administrador de dispositivos** de la lista de resultados.
1. Expandir **Adaptadores de pantalla**. 

Desafortunadamente, la característica de luz nocturna no está disponible si el dispositivo usa un controlador DisplayLink o un controlador de pantalla básico.

La característica de luz noctura usa tecnología de gráficos recientes, por lo que es posible que necesite actualizar el controlador de pantalla:  

- Busque actualizaciones en **Inicio** > **Configuración** > **Actualización y seguridad** > **Windows Update** > **Buscar actualizaciones**.  

O

- Visite el sitio web de soporte técnico de su fabricante de hardware para descargar e instalar manualmente los controladores de visualización más recientes.

## <a name="reset-night-light-in-the-registry"></a>Restablecer la luz nocturna en el registro

Si la actualización del controlador de pantalla no funciona, puede que necesite restablecer la luz nocturna en el registro.  

**Precaución:** Este paso para solucionar problemas solo se recomienda para usuarios expertos. La modificación incorrecta del registro puede producir graves problemas. Para mayor protección, haga copia de seguridad del registro antes de modificarlo para poder restaurarlo si hay problemas.

1. En el cuadro de búsqueda, escriba **Regedit** y, después, seleccione **Editor del Registro** en los resultados de búsqueda.

1. Vaya a la siguiente clave del registro: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exporte y elimine la siguiente subclave:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exporte y elimine la siguiente subclave:$$windows.data.bluelightreduction.settings

1. Reinicie Windows y compruebe si las opciones de luz nocturna están disponibles.


