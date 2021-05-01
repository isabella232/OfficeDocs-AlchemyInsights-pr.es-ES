---
title: Problemas con SharePoint en equipos con Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067014"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemas con SharePoint en equipos con Windows 7

Si experimenta errores en equipos con Windows 7 mientras trabaja en SharePoint o OneDrive, es posible estén relacionados con el desuso de TLS 1.0/1.1. Para más información vea:

- [Preparar TLS 1.2 en Office 365 y CCO de Office 365](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Los clientes de Windows 7 SP1/Windows 8 deben tener TLS1.2 habilitado. Para más información, consulte [Errores de autenticación cuando el cliente no admite TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Instale KB3140245 y cree el valor de registro. Para obtener más información, consulte [Actualizar para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Los clientes de Windows 7 SP1/Windows 8 deben asegurarse de que estén instalados los conjuntos de cifrado TLS más recientes. Para obtener más información, consulte [Advertencia de Seguridad de Microsoft 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


