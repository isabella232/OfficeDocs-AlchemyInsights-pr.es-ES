---
title: Corregir problemas comunes con el formato de registro DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737866"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="83043-102">Corregir problemas comunes con el formato de registro DKIM</span><span class="sxs-lookup"><span data-stu-id="83043-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="83043-103">La mayoría de los problemas de configuración dkim están relacionados con registros DNS incorrectos.</span><span class="sxs-lookup"><span data-stu-id="83043-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="83043-104">Para corregir los problemas de configuración de DKIM, compruebe que el registro DKIM CNAME **(no** un registro TXT) tiene el formato correcto.</span><span class="sxs-lookup"><span data-stu-id="83043-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="83043-105">Para obtener más información, vea [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="83043-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="83043-106">Si necesita ayuda con registros DNS en general, vea [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="83043-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="83043-107">Después de crear o actualizar los registros DNS DKIM en el servicio de hospedaje DNS de su dominio, tendrá que esperar a que se propaguen los registros DNS.</span><span class="sxs-lookup"><span data-stu-id="83043-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
