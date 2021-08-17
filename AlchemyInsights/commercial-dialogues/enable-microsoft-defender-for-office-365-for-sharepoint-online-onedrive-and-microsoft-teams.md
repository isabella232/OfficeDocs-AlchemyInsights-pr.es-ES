---
title: Habilitar Microsoft Defender para Office 365 para SharePoint Online, OneDrive y Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058883"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar Microsoft Defender para Office 365 para SharePoint Online, OneDrive y Microsoft Teams

1. Con sus credenciales de administrador global o de administración de seguridad, inicie sesión en el Centro de seguridad y [cumplimiento Office 365 de seguridad y cumplimiento.](https://protection.office.com/)
2. Seleccione **Administración de amenazas** en el panel izquierdo y, a continuación, seleccione **Directiva** Caja fuerte  >  [datos adjuntos](https://protection.office.com/safeattachment).
3. Seleccione Activar Microsoft Defender para Office 365 para **SharePoint, OneDrive y Microsoft Teams** y, a continuación, **seleccione Guardar**.
    > [!TIP]
    >
    > - Como administrador global o administrador de SharePoint Online, ejecute el siguiente cmdlet de PowerShell con el parámetro **DisallowInfectedFileDownload** establecido en *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurar alertas para archivos detectados](https://go.microsoft.com/fwlink/?linkid=2092110)

Para obtener más información, vea [Microsoft Defender for Office 365 for SharePoint, OneDrive y Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
