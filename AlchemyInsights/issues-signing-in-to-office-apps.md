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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028057"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Corregir el Microsoft 365 de correo electrónico "Lo sentimos, otra cuenta de la organización ya ha iniciado sesión" mensaje

Para corregir este error, siga estos pasos:

- Quite todas las cuentas de trabajo, excepto la cuenta afectada, mediante Windows Configuración > **access work o school**.
- [Borra Office credenciales con](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br/>
    **Nota:** Las rutas de acceso del Office 2016 han cambiado a 16.0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra una Aplicación de Office, elija **Cerrar** sesión de  >  **la cuenta** de  >  **archivo.** A continuación, inicie sesión con una cuenta de usuario con una licencia válida. Para obtener información más detallada, consulte [Cuentas en Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [No se puede iniciar sesión en una aplicación de Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para obtener más información, vea ["Lo sentimos, otra](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)cuenta de la organización ya ha iniciado sesión en este equipo" en Office .