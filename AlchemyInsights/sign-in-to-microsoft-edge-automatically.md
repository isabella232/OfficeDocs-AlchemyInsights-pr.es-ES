---
title: Iniciar sesión en Microsoft Edge automáticamente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599501"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Iniciar sesión en Microsoft Edge automáticamente

Microsoft Edge usa la cuenta predeterminada del sistema operativo para iniciar sesión automáticamente en un usuario de acuerdo con la configuración del dispositivo del usuario. 

A continuación se describen los escenarios de cada tipo de configuración de dispositivo y su proceso de inicio de sesión de usuario dependiente:

1. **El dispositivo es Hybrid/AAD-J**: esta opción está disponible en Windows 10, Windows de bajo nivel y las versiones de servidor correspondientes. Los usuarios inician sesión automáticamente con sus cuentas de Azure Active Directory (AD).
2. **El dispositivo está unido al dominio**: esta opción está disponible en Windows 10, Windows de bajo nivel y las versiones de servidor correspondientes. De forma predeterminada, los usuarios con cuentas de dominio no inician sesión automáticamente; para habilitar el inicio de sesión automático para ellos, use la directiva **ConfigureOnPremisesAccountAutoSignIn** . Para habilitar el inicio de sesión automático para los usuarios con cuentas de Azure AD, piense en unirse a los dispositivos híbridos.
3. **La cuenta predeterminada del sistema operativo es una cuenta de Microsoft**: esta opción está disponible en Windows 10 RS3 (versión 1709, compilación 10.0.16299) y versiones posteriores. Es poco probable que se produzca un escenario en dispositivos empresariales. Sin embargo, si la cuenta predeterminada del sistema operativo es una cuenta de Microsoft, Microsoft Edge iniciará sesión automáticamente en el usuario con la cuenta de Microsoft.
 
 
