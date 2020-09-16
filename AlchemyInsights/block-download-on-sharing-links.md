---
title: Bloquear las descargas en vínculos para compartir
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685759"
---
# <a name="block-download-on-sharing-links"></a>Bloquear las descargas en vínculos para compartir

**Bloquear descargas** está disponible para los **vínculos de solo vista** a los documentos de Office. Si selecciona esta opción, los usuarios que tengan acceso al archivo a través del vínculo que creó no verán las opciones para descargar, imprimir o copiar el archivo.

Los administradores pueden controlar si la configuración de "bloquear descargas" solo aparece para archivos de Office cambiando la configuración `BlockDownloadLinksFileType` en los cmdlets de PowerShell [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) o [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps).
