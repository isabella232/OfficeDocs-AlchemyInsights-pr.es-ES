---
title: Problemas al iniciar sesión en aplicaciones de Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695196"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corrección de las aplicaciones de Microsoft 365 "el módulo de plataforma de confianza del equipo no está funcionando correctamente" mensaje

Para corregir este error, siga estos pasos:

- Instale las actualizaciones más recientes para [Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Borre las credenciales de Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el administrador de credenciales de Windows.<br/>
    **Nota:** Las rutas del registro para Office 2016 han cambiado a 16,0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)
- Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir los errores del módulo de plataforma de confianza (TPM).
- Establezca EnableADAL = 0 mediante los pasos siguientes:  
    1. Haga clic con el botón secundario en el botón Inicio de Windows, elija **Ejecutar**, escriba **regedit**y, a continuación, elija **Aceptar**.
    2. Seleccione **sí** para permitir que el editor del registro realice cambios en el dispositivo.
    3. En el editor del registro, agregue un valor DWORD de **EnableADAL** con un valor de **0** en HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Para obtener más información, vea [problemas de conexión en el inicio de sesión después de actualizar a Office 2016 Build 16.0.7967 en Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).