---
title: Usar perfiles de correo electrónico con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919440"
---
# <a name="using-email-profiles-with-intune"></a>Usar perfiles de correo electrónico con Intune

Intune se puede usar para crear e implementar perfiles de correo electrónico para el cliente de correo electrónico nativo (integrado) en varias plataformas de dispositivos.

Para más información sobre algunas de las restricciones relacionadas con los perfiles de correo electrónico, como la forma en que se controlan la presencia de los perfiles existentes y cómo quitar los perfiles de correo electrónico, consulte [Agregar la configuración de correo electrónico en dispositivos con Intune](https://docs.microsoft.com/intune/email-settings-configure).

Para obtener más información acerca de cómo crear perfiles de correo electrónico para cada plataforma de dispositivo, consulte:

[Configuración de dispositivo Android para configurar el correo electrónico, la autenticación y la sincronización en Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Agregar la configuración de correo electrónico para dispositivos iOS y iPadOS en Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Configuración del perfil de correo electrónico en Microsoft Intune para dispositivos que ejecutan Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Configuración de Perfil de correo electrónico para dispositivos que ejecutan Windows 10 en Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problema común de sincronización**

**Un perfil de correo electrónico KNOX on Android impide que los contactos, el Calendario de Outlook y las tareas de usuario se sincronicen con los dispositivos de usuario.**

El perfil de correo electrónico KNOX on Android KNOX ofrece al administrador la opción de decidir qué tipos de contenido se sincronizan con el dispositivo al establecer cada uno en enabled.

Si la configuración de cualquiera de los tipos de contenido se establece en **No se configura** (predeterminado), el tipo de contenido no se sincronizará automáticamente. Es posible que un usuario habilite el tipo de contenido que quiera directamente en el dispositivo de forma manual, pero que la configuración de directiva de Intune sobrescriba la configuración y se detenga la sincronización de ese tipo de contenido.

