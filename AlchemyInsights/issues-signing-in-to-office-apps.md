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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695340"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Corrección de las aplicaciones de 365 de Microsoft "la otra cuenta de su organización ya ha iniciado sesión" Message

Para corregir este error, siga estos pasos:

- Quite todas las cuentas de trabajo, excepto la cuenta afectada, mediante la configuración de Windows > **acceso a la oficina o a la escuela**.
- [Borre las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el administrador de credenciales de Windows.<br/>
    **Nota:** Las rutas del registro para Office 2016 han cambiado a 16,0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)
- Abra una aplicación de Office y **File**elija la opción  >  **Account**  >  **Cerrar sesión**de la cuenta de archivo. A continuación, inicie sesión con una cuenta de usuario con una licencia válida. Para obtener información más detallada, consulte [Cuentas en Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Para Mac, consulte [No se puede iniciar sesión en una aplicación de Office 2016 para Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Para obtener más información, vea ["lo sentimos, otra cuenta de su organización ya ha iniciado sesión en este equipo" en Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).