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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946632"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Error "Hubo un error al validar el token de acceso" durante la incorporación de Desktop Analytics

Normalmente, este error se observa cuando expira el token de autenticación. Normalmente, la actualización de la página actualiza el token. Sin embargo, este problema puede persistir si hay directivas de acceso condicional aplicadas a la cuenta que se usa para Desktop Analytics integrado. Puede revisar los registros de inicio de sesión de Azure AD en Azure Portal para ver si hay algún error de inicio de sesión para la cuenta que se usa para la incorporación de Desktop Analytics.

Para obtener más información acerca del acceso condicional, visite [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).