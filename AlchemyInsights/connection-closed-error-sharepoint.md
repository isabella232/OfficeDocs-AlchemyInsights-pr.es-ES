---
title: Se ha cerrado la conexión subyacente por error en SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317713"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>"Se ha cerrado la conexión subyacente" por error en SharePoint

Si recibe el error "Se ha cerrado la conexión subyacente" en SharePoint, es posible que se desuso de TLS 1.0/1.1. Para obtener más información, vea estos artículos:

- [Preparar TLS 1.2 en Office 365 y CCO de Office 365](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Se producen errores de autenticación si el cliente no es compatible con TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Actualización para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Si los usuarios utilizan Windows 7, asegúrese de que activen la opción [Conjuntos de cifrado TLS en Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).