---
title: Habilitar Caja fuerte datos adjuntos para SharePoint Online, OneDrive y Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894480"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar Caja fuerte datos adjuntos para SharePoint Online, OneDrive y Microsoft Teams

1. Con sus credenciales de administrador global o de administración de seguridad, abra el portal de Microsoft 365 Defender en y, a continuación, vaya a Directivas & reglas de amenazas Caja fuerte Datos adjuntos en la sección <https://security.microsoft.com>  \>  \>  Directivas 

   Para ir directamente a la **página Caja fuerte datos adjuntos,** use <https://security.microsoft.com/safeattachmentv2> .

2. En la **página Caja fuerte datos adjuntos,** haga clic en **Configuración global**.
3. En el menú desplegable que aparece, seleccione Activar Microsoft Defender para Office 365 para **SharePoint,** OneDrive y Microsoft Teams y, a continuación, **seleccione Guardar**.

    > [!TIP]
    >
    > Siga estos pasos para mejorar la protección de Caja fuerte datos adjuntos para SharePoint, OneDrive y Microsoft Teams:
    >
    > - Para evitar que los usuarios descarguen archivos malintencionados, use el valor del parámetro `$true` *DisallowInfectedFileDownload* en el cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** en SharePoint PowerShell en línea. Para obtener más información, [vea Use SharePoint Online PowerShell to prevent users from downloading malicious files](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    > - [Crear una directiva de alerta para archivos detectados](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Para obtener más información, vea [Caja fuerte Attachments for Office 365 for SharePoint, OneDrive y Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
