---
title: Corrección de las aplicaciones de Microsoft 365 la cuenta está en un mensaje de estado incorrecto
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744562"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Corrección del error "la cuenta de Microsoft 365 apps" tiene un estado incorrecto

Para solucionar este error, pruebe las siguientes opciones en el equipo afectado:

- Abra una aplicación de Office, **File**seleccione Cerrar sesión en la  >  **cuenta**  >  **de archivo de todas las cuentas**. Vuelva a iniciar sesión con una cuenta de usuario que tenga una licencia válida. Para obtener información detallada, consulte [Cuentas en Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Borre las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el administrador de credenciales de Windows.<br>
  **Nota:** Las rutas del registro para Office 2016 han cambiado a 16,0. Por ejemplo, \Software\Microsoft\Office\16.0\Common\Identity\
- Si el error se produce al conectar con Office 365 mediante Office 2013, [habilite la autenticación moderna](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) para el cliente de Office.

Para obtener más información, vea [cómo solucionar problemas de aplicaciones que no son de explorador que no pueden iniciar sesión en Microsoft 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

