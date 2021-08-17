---
title: Inicie sesión para Microsoft Edge automáticamente
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050711"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Inicie sesión para Microsoft Edge automáticamente

Microsoft Edge la cuenta predeterminada del sistema operativo para iniciar sesión automáticamente en un usuario de acuerdo con la configuración del dispositivo del usuario. 

A continuación se describen los escenarios de cada tipo de configuración de dispositivo y su proceso de inicio de sesión de usuario dependiente:

- **El dispositivo es híbrido/AAD-J:** esta opción está disponible en Windows 10 versiones de servidor Windows nivel inferior y en las versiones de servidor correspondientes. Los usuarios iniciaron sesión automáticamente con sus Azure Active Directory (AD)cuentas.
- **El dispositivo está unido a un** dominio: esta opción está disponible en Windows 10, versiones de nivel inferior Windows versiones de servidor correspondientes. De forma predeterminada, los usuarios con cuentas de dominio no han iniciado sesión automáticamente; para habilitar el inicio de sesión automático para ellos, use la **directiva ConfigureOnPremisesAccountAutoSignIn.** Para habilitar el inicio de sesión automático para los usuarios con cuentas de Azure AD, considere la posibilidad de unir híbridos a sus dispositivos.
- La cuenta predeterminada del sistema operativo es una cuenta **microsoft:** esta opción está disponible en Windows 10 RS3 (versión 1709, compilación 10.0.16299) y versiones posteriores. Es poco probable que el escenario se produzca en dispositivos empresariales. Sin embargo, si la cuenta predeterminada del sistema operativo es una cuenta de Microsoft, Microsoft Edge iniciará sesión automáticamente en el usuario con la cuenta de Microsoft.
 
 
