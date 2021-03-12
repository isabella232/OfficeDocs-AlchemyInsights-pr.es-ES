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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737348"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar Microsoft Defender para Office 365 para SharePoint Online, OneDrive y Microsoft Teams

1. Con sus credenciales de administrador global o de administración de seguridad, inicie sesión en el Centro de seguridad y cumplimiento de [Office 365](https://protection.office.com/).
2. Seleccione **Administración de amenazas** en el panel izquierdo y, a continuación, seleccione Datos   >  [adjuntos seguros de directivas.](https://protection.office.com/safeattachment)
3. Seleccione **Activar Microsoft Defender para Office 365 para SharePoint, OneDrive** y Microsoft Teams y, a continuación, seleccione **Guardar**.
    > [!TIP]
    >
    > - Como administrador global o administrador de SharePoint Online, ejecute el siguiente cmdlet de PowerShell con el parámetro **DisallowInfectedFileDownload** establecido en *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurar alertas para archivos detectados](https://go.microsoft.com/fwlink/?linkid=2092110)

Para obtener más información, vea [Microsoft Defender para Office 365 para SharePoint, OneDrive y Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
