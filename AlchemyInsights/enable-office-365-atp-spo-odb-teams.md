---
title: Habilitar Office 365 ATP para SharePoint, OneDrive y Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543945"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitar Microsoft Defender para Office 365 para SharePoint Online, OneDrive y Microsoft Teams

1. Vaya a https://protection.office.com e inicie sesión.
2. Elija **Directiva de administración**  >  **de** amenazas Caja fuerte datos  >  **adjuntos**.
3. Seleccione Activar Defender para Office 365 para **SharePoint, OneDrive y Microsoft Teams** y, a continuación, haga clic en **Guardar**.
4. (Recomendado) Como administrador global o administrador de SharePoint Online, ejecute el cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con el parámetro **DisallowInfectedFileDownload** establecido en *true*.
5. (Recomendado) [Configurar alertas para](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) archivos detectados.

> [!NOTE]
> Microsoft Defender para Office 365 examinará todos los archivos de SharePoint Online, OneDrive o Microsoft Teams. Los archivos se examinan de forma asincrónica, a través de un proceso que usa eventos de actividad de invitado y uso compartido, junto con heurística inteligente y señales de amenazas para identificar archivos malintencionados. Consulta [Microsoft Defender para Office 365 para SharePoint, OneDrive y Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).