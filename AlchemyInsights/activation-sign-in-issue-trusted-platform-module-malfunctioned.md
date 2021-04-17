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
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822904"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Corregir las aplicaciones de Microsoft 365 Mensaje "El módulo de plataforma de confianza del equipo no funciona correctamente"

Para corregir este error, siga estos pasos:

1. Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes.   
2. Con las cuentas **de**  >  **configuración de**  >  **Windows, & cuentas de correo** electrónico, quita las cuentas de trabajo existentes. 
3. Con Configuración **de** Windows  >  **Cuentas** Acceso a  >  **trabajo o escuela,** desconecte las cuentas existentes. 
4. Restablezca el estado de activación de Office [Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir errores del Módulo de plataforma segura (TPM).