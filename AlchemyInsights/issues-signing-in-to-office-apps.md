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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833092"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Corregir las aplicaciones de Microsoft 365 "Lo sentimos, otra cuenta de la organización ya ha iniciado sesión" mensaje

Para corregir este error, siga estos pasos:

- Quita todas las cuentas de trabajo, excepto la cuenta afectada, con configuración de Windows > **acceso a trabajo o escuela**.
- [Borra las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el Administrador de credenciales de Windows.<br/>
    **Nota:** Las rutas de acceso del Registro para Office 2016 han cambiado a 16.0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra una aplicación de Office, elija **Cerrar** sesión de  >  **la**  >  **cuenta de archivo**. A continuación, inicie sesión con una cuenta de usuario con una licencia válida. Para obtener información más detallada, consulte [Cuentas en Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [No se puede iniciar sesión en una aplicación de Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para obtener más información, vea ["Lo sentimos, otra cuenta de su organización ya ha iniciado](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)sesión en este equipo" en Office .