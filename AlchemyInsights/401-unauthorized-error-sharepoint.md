---
title: 401 Error no autorizado en SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890283"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Error no autorizado en SharePoint

Si recibe el error "(401) No autorizado" en SharePoint, es posible que esté relacionado con el desuso de TLS 1.0/1.1. Para obtener más información, vea:

- [Preparar TLS 1.2 en Office 365 y CCO de Office 365](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Se producen errores de autenticación si el cliente no es compatible con TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Actualización para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Si los usuarios utilizan Windows 7, asegúrese de que activen la opción [Conjuntos de cifrado TLS en Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).