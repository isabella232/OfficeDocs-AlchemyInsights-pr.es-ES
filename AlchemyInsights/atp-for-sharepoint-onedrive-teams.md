---
title: Microsoft Defender para Office 365 para SharePoint, OneDrive y Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543594"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender para Office 365 para SharePoint, OneDrive y Microsoft Teams

Siga estos pasos para habilitar Microsoft Defender para Office 365:

1. Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.

2. En el panel de navegación izquierdo en **Administración de amenazas,** elija **Directiva** Caja fuerte \> **datos adjuntos**.

3. Seleccione **Activar Defender para Office 365 para SharePoint, OneDrive y Microsoft Teams**.

4. [Cree una directiva de alerta de actividad](/microsoft-365/compliance/create-activity-alerts) para recibir notificaciones cuando detectemos archivos malintencionados.

Para obtener instrucciones completas, vea este artículo Activar Caja fuerte datos adjuntos para [SharePoint, OneDrive y Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Nota:** Por diseño, Microsoft Defender para Office 365 no analiza todos los archivos de SharePoint Online, OneDrive para la Empresa o Microsoft Teams. Los archivos se examinan de forma asincrónica mediante un proceso que usa la actividad de uso compartido, la actividad de invitado y las señales de amenaza para identificar archivos malintencionados. Para obtener más información, [vea Caja fuerte attachments for SharePoint, OneDrive y Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
