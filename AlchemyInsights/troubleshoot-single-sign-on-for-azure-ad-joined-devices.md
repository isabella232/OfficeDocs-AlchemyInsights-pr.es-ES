---
title: Solucionar problemas de inicio de sesión único para dispositivos unidos a Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039263"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Solucionar problemas de inicio de sesión único para dispositivos unidos a Azure AD

Si tiene un entorno de Active Directory (AD) local y desea unir los equipos unidos a un dominio de AD a Azure AD, puede hacerlo mediante la combinación híbrida de Azure AD. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) proporciona los pasos relacionados para implementar una combinación híbrida de Azure AD en su entorno.

Para obtener más información, vea [Configure Azure AD joined devices for Single-Sign On](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)on using Windows Hello for Business .

**Problemas del token de actualización principal (PRT)**

Un token de actualización principal (PRT) es un artefacto clave de la autenticación de Azure AD en dispositivos Windows 10, Windows Server 2016 versiones posteriores, iOS y Android. Se trata de un token web JSON (JWT) especialmente emitido a los agentes de tokens de microsoft para habilitar el inicio de sesión único (SSO) en todas las aplicaciones usadas en esos dispositivos. Para obtener información detallada sobre cómo se emite, usa y protege un PRT en dispositivos Windows 10, vea ¿Qué es un token de actualización [principal?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES y AzureADPrt: SÍ**

Estos campos indican si el usuario se ha autenticado correctamente en Azure AD al iniciar sesión en el dispositivo. Si los valores **son NO,** podría deberse a:

- Clave de almacenamiento mal en el TPM asociado con el dispositivo al registrarse (compruebe keySignTest mientras se ejecuta con privilegios elevados)
- Identificador de inicio de sesión alternativo
- Proxy HTTP no encontrado

Para solucionar problemas de dispositivos mediante el comando dsregcmd, consulte [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
