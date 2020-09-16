---
title: Enviar notificaciones personalizadas con Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720663"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cómo enviar notificaciones personalizadas a los usuarios de dispositivos administrados iOS y Android

Las notificaciones personalizadas para Intune las procesa la aplicación portal de empresa en el dispositivo de un usuario. A continuación, la aplicación crea la notificación de inserción en ese dispositivo.

Los siguientes son requisitos previos de dispositivos para admitir la recepción de notificaciones personalizadas, y para que la aplicación cree la notificación de inserción:

- El dispositivo debe tener instalada la aplicación portal de empresa.  

- El dispositivo debe permitir que la aplicación de portal de empresa envíe notificaciones de inserción. Cuando la aplicación se instale o actualice, se le pedirá al usuario que permita las notificaciones.

- Los dispositivos Android deben tener instalado Google Play Services.

- El dispositivo debe estar inscrito con Intune.

Para obtener más información, incluido cómo enviar un mensaje, consulte la documentación de la [característica](https://docs.microsoft.com/intune/custom-notifications).
