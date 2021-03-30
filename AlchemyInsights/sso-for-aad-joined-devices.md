---
title: Single-Sign para dispositivos unidos a Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403831"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Inicio de sesión único para dispositivos unidos a Azure Active Directory

Si tiene un entorno de Active Directory (AD) local y desea unir los equipos unidos a un dominio de AD a Azure AD, puede hacerlo mediante la combinación híbrida de Azure AD. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Configurar dispositivos unidos a Azure AD para dispositivos locales Single-Sign En el uso de Windows Hello para empresas](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

Problemas del token de actualización **principal (PRT)** Un token de actualización principal (PRT) es un artefacto clave de la autenticación de Azure AD en windows 10, Windows Server 2016 y versiones posteriores, dispositivos iOS y Android. Se trata de un token web JSON (JWT) especialmente emitido a los agentes de tokens de microsoft para habilitar el inicio de sesión único (SSO) en todas las aplicaciones usadas en esos dispositivos. [In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.

**WamDefaultSet: YES y AzureADPrt: SÍ** Estos campos indican si el usuario se ha autenticado correctamente en Azure AD al iniciar sesión en el dispositivo. Si los valores son **NO,** podría deberse a:

- Clave de almacenamiento mala en el TPM asociado con el dispositivo al registrarse (comprueba KeySignTest mientras se ejecuta con privilegios elevados).
- Identificador de inicio de sesión alternativo
- Proxy HTTP no encontrado

Solucionar problemas de dispositivos mediante el comando dsregcmd: [estado de SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
