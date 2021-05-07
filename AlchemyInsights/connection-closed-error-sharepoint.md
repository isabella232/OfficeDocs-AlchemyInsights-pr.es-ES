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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233443"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="b58e7-102">"Se ha cerrado la conexión subyacente" por error en SharePoint</span><span class="sxs-lookup"><span data-stu-id="b58e7-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="b58e7-p101">Si recibe el error "Se ha cerrado la conexión subyacente" en SharePoint, es posible que se desuso de TLS 1.0/1.1. Para obtener más información, vea estos artículos:</span><span class="sxs-lookup"><span data-stu-id="b58e7-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="b58e7-105">Preparar TLS 1.2 en Office 365 y CCO de Office 365</span><span class="sxs-lookup"><span data-stu-id="b58e7-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="b58e7-106">Se producen errores de autenticación si el cliente no es compatible con TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="b58e7-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="b58e7-107">Si los usuarios utilizan Windows 7, asegúrese de que activen la opción [Conjuntos de cifrado TLS en Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="b58e7-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>