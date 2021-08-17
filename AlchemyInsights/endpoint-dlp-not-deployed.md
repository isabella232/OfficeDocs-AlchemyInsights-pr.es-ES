---
title: DLP en punto de conexión no implementado en el dispositivo del usuario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 2d5f0486ed8d4cbd95603f223bc0e48c4dcf38abb001d1616ca968b1d6bba7de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044249"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP en punto de conexión no implementado en el dispositivo del usuario

Si la configuración de prevención de pérdida de datos (DLP) en punto de conexión no se ha aplicado en el dispositivo de un usuario, confirme que cumple estos requisitos:

- La compilación 1809 o posterior de Windows 10 x64 está instalada en el dispositivo.
- Está instalada la versión 4.18.2009.7 o una posterior del cliente antimalware.
- El dispositivo cumple **una** de las siguientes opciones:
    
    - Unido a Azure Active Directory (Azure AD)
    - Unido a Azure AD híbrido 
    - Registrado en AAD

- Para aplicar acciones de directiva, asegúrese de que el explorador Microsoft Chromium Edge está instalado en el dispositivo de punto de conexión.

Para ver los requisitos adicionales para implementar DLP en punto de conexión, vea [Introducción a la Prevención de pérdida de datos en punto de conexión](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).