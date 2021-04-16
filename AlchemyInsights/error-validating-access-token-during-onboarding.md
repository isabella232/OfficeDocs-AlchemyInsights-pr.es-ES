---
title: Se produjo un error al validar el error de token de acceso durante el abordaje de Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813705"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="79855-102">Error "Hubo un error al validar el token de acceso" durante la incorporación de Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="79855-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="79855-103">Normalmente, este error se observa cuando expira el token de autenticación.</span><span class="sxs-lookup"><span data-stu-id="79855-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="79855-104">Normalmente, la actualización de la página actualiza el token.</span><span class="sxs-lookup"><span data-stu-id="79855-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="79855-105">Sin embargo, este problema puede persistir si hay directivas de acceso condicional aplicadas a la cuenta que se usa para Desktop Analytics integrado.</span><span class="sxs-lookup"><span data-stu-id="79855-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="79855-106">Puede revisar los registros de inicio de sesión de Azure AD en Azure Portal para ver si hay algún error de inicio de sesión para la cuenta que se usa para la incorporación de Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="79855-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="79855-107">Para obtener más información acerca del acceso condicional, visite [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="79855-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>