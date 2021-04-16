---
title: Corregir las aplicaciones de Microsoft 365 Su cuenta está en un mensaje de estado malo
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812553"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Corregir el error de aplicaciones de Microsoft 365 "Su cuenta está en mal estado"

Para corregir este error, pruebe las siguientes opciones en el equipo afectado:

- Abra una aplicación de Office, **seleccione Cerrar** sesión de la  >  **cuenta**  >  **de archivo de todas las cuentas.** Vuelva a iniciar sesión con una cuenta de usuario que tenga una licencia válida. Para obtener información detallada, consulte [Cuentas en Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Borra las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el Administrador de credenciales de Windows.<br>
  **Nota:** Las rutas de acceso del Registro para Office 2016 han cambiado a 16.0. Por ejemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- Si el error se produce al conectarse a Office 365 con Office 2013, habilite la [autenticación](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) moderna para el cliente de Office.

Para obtener más información, vea [How to troubleshoot non-browser apps that can't sign in to Microsoft 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

