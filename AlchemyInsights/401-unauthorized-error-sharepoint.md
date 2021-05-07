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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233530"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Error no autorizado en SharePoint

Si recibe el error "(401) No autorizado" en SharePoint, es posible que esté relacionado con el desuso de TLS 1.0/1.1. Para obtener más información, vea:

[Preparar TLS 1.2 en Office 365 y CCO de Office 365](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Se producen errores de autenticación si el cliente no es compatible con TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Si los usuarios utilizan Windows 7, asegúrese de que activen la opción [Conjuntos de cifrado TLS en Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).