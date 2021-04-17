---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820195"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="09a5b-102">Bloqueo de la autenticación heredada</span><span class="sxs-lookup"><span data-stu-id="09a5b-102">Blocking legacy authentication</span></span>

<span data-ttu-id="09a5b-103">La autenticación heredada es un término que hace referencia a una solicitud de autenticación realizada por:</span><span class="sxs-lookup"><span data-stu-id="09a5b-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="09a5b-104">Clientes de Office antiguos que no usan la autenticación moderna (por ejemplo, cliente de Office 2010).</span><span class="sxs-lookup"><span data-stu-id="09a5b-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="09a5b-105">Cualquier cliente que use protocolos de correo heredados como IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="09a5b-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="09a5b-106">Para obtener más información sobre cómo bloquear la autenticación heredada y habilitar la autenticación moderna, consulte [Bloqueo de la autenticación heredada.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="09a5b-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="09a5b-107">Los valores predeterminados de seguridad en Azure Active Directory (Azure AD) facilitan la seguridad y ayudan a proteger la organización.</span><span class="sxs-lookup"><span data-stu-id="09a5b-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="09a5b-108">Los valores predeterminados de seguridad contienen opciones de seguridad preconfiguradas para ataques comunes.</span><span class="sxs-lookup"><span data-stu-id="09a5b-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="09a5b-109">Para obtener más información acerca de los valores predeterminados de seguridad, consulte [¿Cuáles son los valores predeterminados de seguridad?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="09a5b-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="09a5b-110">**Nota:** Si el espacio empresarial se creó el 22 de octubre de 2019 o después de él, es posible que experimente el nuevo comportamiento seguro de forma predeterminada y ya tenga los valores predeterminados de seguridad habilitados en el espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="09a5b-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="09a5b-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span><span class="sxs-lookup"><span data-stu-id="09a5b-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
