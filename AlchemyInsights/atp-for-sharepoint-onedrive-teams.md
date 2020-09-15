---
title: ATP para SharePoint, OneDrive y Microsoft Teams
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715578"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP para SharePoint, OneDrive y Microsoft Teams

Siga estos pasos para habilitar la protección contra amenazas avanzada:

1. Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.

2. En el panel de navegación izquierdo, en **Administración de amenazas**, elija **Policy** \> **datos adjuntos seguros**de directiva.

3. Seleccione **Activar ATP para SharePoint, OneDrive y Microsoft Teams**.

4. [Cree una directiva de alerta de actividad](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) para recibir notificaciones cuando detecte archivos malintencionados.

Para obtener instrucciones completas, vea este [tema](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Nota**: por diseño, ATP no explora todos los archivos en SharePoint Online, OneDrive para la empresa o Microsoft Teams. Un proceso que usa la actividad de uso compartido, la actividad de invitado y las señales de amenaza para identificar archivos malintencionados se examinan de forma asincrónica. Para obtener más información, vea este [tema](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
