---
title: Single-Sign para dispositivos Azure Active Directory unidos
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050027"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Inicio de sesión único para dispositivos Azure Active Directory unidos

Si tiene un entorno de Active Directory (AD) local y desea unir los equipos unidos a un dominio de AD a Azure AD, puede hacerlo mediante la combinación híbrida de Azure AD. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) proporciona los pasos relacionados para implementar una combinación híbrida de Azure AD en su entorno.

[Configurar dispositivos unidos a Azure AD para aplicaciones locales Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

Problemas del token de actualización **principal (PRT)** Un token de actualización principal (PRT) es un artefacto clave de la autenticación de Azure AD en dispositivos Windows 10, Windows Server 2016 versiones posteriores, iOS y Android. Se trata de un token web JSON (JWT) especialmente emitido a los agentes de tokens de microsoft para habilitar el inicio de sesión único (SSO) en todas las aplicaciones usadas en esos dispositivos. [In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.

**WamDefaultSet: YES y AzureADPrt: SÍ** Estos campos indican si el usuario se ha autenticado correctamente en Azure AD al iniciar sesión en el dispositivo. Si los valores son **NO,** podría deberse a:

- Clave de almacenamiento mala en el TPM asociado con el dispositivo al registrarse (comprueba KeySignTest mientras se ejecuta con privilegios elevados).
- Identificador de inicio de sesión alternativo
- Proxy HTTP no encontrado

Solucionar problemas de dispositivos mediante el comando dsregcmd: [estado de SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
