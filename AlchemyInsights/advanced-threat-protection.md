---
title: Microsoft Defender para Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: 61236d1e0174248cdb49284d6c6c7d49df51e7e9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315095"
---
# <a name="microsoft-defender-for-office-365"></a>Microsoft Defender para Office 365

- Caja fuerte Los datos adjuntos, Caja fuerte vínculos y la suplantación de identidad son parte de Microsoft Defender para Office 365. Enterprise E5, Education A5 y Microsoft 365 Empresa Premium Microsoft Defender para Office 365. Todos los demás planes requieren un complemento de Microsoft Defender para Office 365 suscripción.

- Debe asignar las licencias adecuadas para proteger a los usuarios mediante Microsoft Defender para Office 365. Consulte [Agregar usuarios y asignar licencias al mismo](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) tiempo para obtener instrucciones sobre cómo aplicar licencias masivas a los usuarios.

- Los administradores globales o los administradores de seguridad pueden acceder a Microsoft Defender para obtener Office 365 características en el portal de Microsoft 365 Defender en la sección De colaboración de correo **electrónico &** Directivas \> **& reglas** \> **de** amenazas .

- Caja fuerte Los datos adjuntos Caja fuerte las directivas de vínculos pueden tener ámbito para dominios específicos, miembros de grupo o usuarios individuales. También puede especificar excepciones a las directivas Caja fuerte datos adjuntos y Caja fuerte vínculos basados en el dominio, la pertenencia a grupos o usuarios individuales.

- No hay ninguna directiva predeterminada Caja fuerte datos adjuntos que proteja los mensajes de correo electrónico. Debe crear una [directiva para la](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-attachments-policies) protección Caja fuerte datos adjuntos en el correo electrónico.

  Caja fuerte Los datos adjuntos SharePoint, OneDrive y Microsoft Teams están habilitados o deshabilitados globalmente, y no requieren directivas Caja fuerte datos adjuntos. Para obtener más información, [vea Caja fuerte attachments for SharePoint, OneDrive y Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/mdo-for-spo-odb-and-teams).

- No hay ninguna directiva de vínculos Caja fuerte predeterminada que proteja los mensajes de correo electrónico o Microsoft Teams. Debe crear una [directiva para la](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies) protección de Caja fuerte vínculos en el correo electrónico y Teams.

  Caja fuerte La protección de vínculos para Office 365 aplicaciones se aplica a todos los usuarios de la organización con licencia para Defender para Office 365, independientemente de si los usuarios se incluyen en directivas de vínculos de Caja fuerte activas o no. Para obtener más información, [consulta Caja fuerte configuración de vínculos para Office 365 aplicaciones](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links#safe-links-settings-for-office-365-apps).
