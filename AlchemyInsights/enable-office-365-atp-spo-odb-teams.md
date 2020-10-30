---
title: Habilitación de Office 365 ATP para SharePoint, OneDrive y Microsoft Teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801092"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Habilitación de Microsoft defender para Office 365 para SharePoint Online, OneDrive y Microsoft Teams

1. Vaya a https://protection.office.com e inicie sesión.
2. Seleccione Directiva de **Administración de amenazas**  >  **Policy**  >  : **datos adjuntos seguros** .
3. Seleccione **Activar ATP para SharePoint, OneDrive y Microsoft Teams** y, a continuación, haga clic en **Guardar** .
4. Recomenda Como administrador global o administrador de SharePoint Online, ejecute el cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con el parámetro **DisallowInfectedFileDownload** establecido en *true* .
5. Recomenda [Configurar alertas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para los archivos detectados.

> [!NOTE]
> ATP detendrá la exploración de todos los archivos en SharePoint Online, OneDrive o Microsoft Teams. Los archivos se examinan de forma asincrónica, a través de un proceso que usa eventos de actividad de uso compartido e invitados, junto con heurística inteligente y señales de amenazas para identificar archivos malintencionados. Consulte [ATP para SharePoint, OneDrive y Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).