---
title: 'Problema de activación/inicio de sesión: el módulo de plataforma de confianza no funciona correctamente'
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
- "3406"
- "9001429"
ms.openlocfilehash: 90fc3135dcde5073330abb7cfe0e45c799e2154d9cd27c075c2c9ac89c18a641
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937298"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corregir el Microsoft 365 de aplicaciones de confianza "El módulo de plataforma de confianza del equipo no funciona correctamente" mensaje

Para corregir este error, siga estos pasos:

1. Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes.   
2. Con Windows **Configuración** cuentas de  >    >  **correo & cuentas** de correo electrónico , quite las cuentas de trabajo existentes. 
3. Con Windows **Configuración** acceso a cuentas  >  **laborales** o  >  **educativas**, desconecte las cuentas existentes. 
4. Restablezca el estado de activación de Office [Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir errores del Módulo de plataforma segura (TPM).