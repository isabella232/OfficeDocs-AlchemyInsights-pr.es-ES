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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086181"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cómo enviar notificaciones personalizadas a los usuarios de dispositivos iOS y Android administrados

Las notificaciones personalizadas para Intune las procesa la Portal de empresa en el dispositivo de un usuario. A continuación, la aplicación crea la notificación de inserción en ese dispositivo.

A continuación se indican los requisitos previos del dispositivo para admitir la recepción de notificaciones personalizadas y para que la aplicación cree la notificación de inserción:

- El dispositivo debe tener instalada Portal de empresa aplicación.  

- El dispositivo debe permitir que Portal de empresa aplicación envíe notificaciones de inserción. Cuando la aplicación se instala o actualiza, se le pedirá al usuario que permita las notificaciones.

- Los dispositivos Android deben tener instalado Google Play Services.

- El dispositivo debe estar inscrito en Intune.

Para obtener más información, incluido cómo enviar un mensaje, consulte la [documentación de características](https://docs.microsoft.com/intune/custom-notifications).
