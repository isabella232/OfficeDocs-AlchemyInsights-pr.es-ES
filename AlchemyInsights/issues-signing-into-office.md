---
title: Problemas al iniciar sesión en Microsoft 365 aplicaciones
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744663"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemas al iniciar sesión Aplicaciones Microsoft 365

Nota: Si usa una versión anterior de Windows (por ejemplo, Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), use la corrección fácil para habilitar TLS 1.2 de forma predeterminada. Para obtener más información, consulte [Actualizar para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Para solucionar los problemas de inicio de sesión con las aplicaciones de Microsoft 365, pruebe las siguientes opciones en el equipo afectado:  

- Para Windows, consulte [Recomendaciones sobre la resolución de problemas comunes de inicio de sesión](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Para Mac, consulta [No se puede iniciar sesión en una Office 2016 para Mac aplicación](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Sugerencia** en equipos Windows, podemos diagnosticar y solucionar varios problemas comunes de inicio de sesión de Office. Descargue y ejecute el **[Asistente de soporte y recuperación de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nuestra herramienta automatizada.

**Nota:** No se recomienda deshabilitar la autenticación moderna (ADAL) o la administración de cuentas web (WAM) para solucionar problemas de inicio de sesión o **activación.** Si los errores se producen al conectarse a Microsoft 365 con Office 2013, asegúrese de habilitar la autenticación moderna para Office cliente. [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Para ver acciones de solución de problemas específicas, vea:

[Problemas de conexión al iniciar sesión después de actualizar a Office 2016, compilación 16.0.7967 en Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[No puede iniciar sesión en su cuenta organizativa, como Office 365, Azure o Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Cómo solucionar problemas de aplicaciones que no son del explorador que no pueden iniciar sesión en Office 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Se solicitan repetidamente credenciales en Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)