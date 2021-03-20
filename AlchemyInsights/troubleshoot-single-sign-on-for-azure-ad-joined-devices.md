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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898087"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Solucionar problemas de inicio de sesión único para dispositivos unidos a Azure AD

Si tiene un entorno de Active Directory (AD) local y desea unir los equipos unidos a un dominio de AD a Azure AD, puede hacerlo mediante la combinación híbrida de Azure AD. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

Para obtener más información, vea [Configure Azure AD joined devices for Single-Sign On](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)on using Windows Hello for Business .

**Problemas del token de actualización principal (PRT)**

Un token de actualización principal (PRT) es un artefacto clave de la autenticación de Azure AD en windows 10, Windows Server 2016 y versiones posteriores, dispositivos iOS y Android. Se trata de un token web JSON (JWT) especialmente emitido a los agentes de tokens de microsoft para habilitar el inicio de sesión único (SSO) en todas las aplicaciones usadas en esos dispositivos. Para obtener más información sobre cómo se emite, usa y protege un PRT en dispositivos Windows 10, consulta ¿Qué es un token de actualización [principal?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES y AzureADPrt: SÍ**

Estos campos indican si el usuario se ha autenticado correctamente en Azure AD al iniciar sesión en el dispositivo. Si los valores **son NO,** podría deberse a:

- Clave de almacenamiento mal en el TPM asociado con el dispositivo al registrarse (compruebe keySignTest mientras se ejecuta con privilegios elevados)
- Identificador de inicio de sesión alternativo
- Proxy HTTP no encontrado

Para solucionar problemas de dispositivos mediante el comando dsregcmd, consulte [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
