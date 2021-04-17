---
title: Problemas al iniciar sesión en aplicaciones de Microsoft 365
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
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833032"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corregir las aplicaciones de Microsoft 365 Mensaje "El módulo de plataforma de confianza del equipo no funciona correctamente"

Para corregir este error, siga estos pasos:

- Instalar las actualizaciones más recientes [para Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Borra las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) con el Administrador de credenciales de Windows.<br/>
    **Nota:** Las rutas de acceso del Registro para Office 2016 han cambiado a 16.0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)
- Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir errores del Módulo de plataforma segura (TPM).
- Establezca EnableADAL = 0 siguiendo los pasos siguientes:  
    1. Haga clic con el botón secundario en el botón Inicio de Windows, elija **Ejecutar**, escriba **regedit** y, a continuación, elija **Aceptar**.
    2. Selecciona **Sí** para permitir que el Editor del Registro realice cambios en el dispositivo.
    3. En el Editor del Registro, agregue un valor DWORD de **EnableADAL** con una configuración de **0** en HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Para obtener más información, vea [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).