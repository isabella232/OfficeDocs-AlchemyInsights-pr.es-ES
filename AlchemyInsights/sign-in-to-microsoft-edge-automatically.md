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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398746"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Iniciar sesión en Microsoft Edge automáticamente

Microsoft Edge usa la cuenta predeterminada del sistema operativo para iniciar sesión automáticamente en un usuario de acuerdo con la configuración del dispositivo del usuario. 

A continuación se describen los escenarios de cada tipo de configuración de dispositivo y su proceso de inicio de sesión de usuario dependiente:

- **El dispositivo es híbrido/AAD-J:** esta opción está disponible en Windows 10, Windows de nivel inferior y las versiones de servidor correspondientes. Los usuarios inician sesión automáticamente con sus cuentas de Azure Active Directory (AD).
- **El dispositivo está unido a un** dominio: esta opción está disponible en Windows 10, Windows de nivel inferior y las versiones de servidor correspondientes. De forma predeterminada, los usuarios con cuentas de dominio no han iniciado sesión automáticamente; para habilitar el inicio de sesión automático para ellos, use la **directiva ConfigureOnPremisesAccountAutoSignIn.** Para habilitar el inicio de sesión automático para los usuarios con cuentas de Azure AD, considere la posibilidad de unir híbridos a sus dispositivos.
- La cuenta predeterminada del sistema operativo es una cuenta **de Microsoft:** esta opción está disponible en Windows 10 RS3 (versión 1709, compilación 10.0.16299) y versiones posteriores. Es poco probable que el escenario se produzca en dispositivos empresariales. Sin embargo, si la cuenta predeterminada del sistema operativo es una cuenta de Microsoft, Microsoft Edge iniciará sesión automáticamente en el usuario con la cuenta de Microsoft.
 
 
