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
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919044"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Error no autorizado en SharePoint

Si recibe el error "(401) No autorizado" en SharePoint, es posible que esté relacionado con el desuso de TLS 1.0/1.1. Para obtener más información, vea:

- [Preparar TLS 1.2 en Office 365 y CCO de Office 365](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Se producen errores de autenticación si el cliente no es compatible con TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Actualización para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Si los usuarios utilizan Windows 7, asegúrese de que activen la opción [Conjuntos de cifrado TLS en Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).