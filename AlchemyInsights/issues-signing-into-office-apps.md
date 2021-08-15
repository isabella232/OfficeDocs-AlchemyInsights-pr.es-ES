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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986908"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corregir el Microsoft 365 de aplicaciones de confianza "El módulo de plataforma de confianza del equipo no funciona correctamente" mensaje

Para corregir este error, siga estos pasos:

- Instale las actualizaciones más recientes [para Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Borra Office credenciales con](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br/>
    **Nota:** Las rutas de acceso del Office 2016 han cambiado a 16.0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)
- Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir errores del Módulo de plataforma segura (TPM).
- Establezca EnableADAL = 0 siguiendo los pasos siguientes:  
    1. Haga clic con el botón Windows botón Inicio, elija **Ejecutar**, **escriba regedit** y, a continuación, **elija Aceptar**.
    2. Selecciona **Sí** para permitir que el Editor del Registro realice cambios en el dispositivo.
    3. En el Editor del Registro, agregue un valor DWORD de **EnableADAL** con una configuración de **0** en HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para obtener más información, vea Connection [issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).