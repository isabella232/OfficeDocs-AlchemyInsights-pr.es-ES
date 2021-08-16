---
title: Corrección de Microsoft 365 aplicaciones Su cuenta está en un mensaje de estado malo
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
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068253"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Corregir el error Microsoft 365 aplicaciones de correo electrónico "Su cuenta está en mal estado"

Para corregir este error, pruebe las siguientes opciones en el equipo afectado:

- Abra una Aplicación de Office, seleccione **Cerrar** sesión de la  >  **cuenta**  >  **de archivo de todas las cuentas**. Vuelva a iniciar sesión con una cuenta de usuario que tenga una licencia válida. Para obtener información detallada, consulte [Cuentas en Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Borra Office credenciales con](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br>
  **Nota:** Las rutas de acceso del Office 2016 han cambiado a 16.0. Por ejemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- Si el error se produce al conectarse a Office 365 con Office [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 2013, habilite la autenticación moderna para el Office cliente.

Para obtener más información, vea [How to troubleshoot non-browser apps that can't sign in to Microsoft 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

