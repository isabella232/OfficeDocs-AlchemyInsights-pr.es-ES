---
title: Complemento de Teams para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582087"
---
# <a name="teams-add-in-for-mac"></a>Complemento de Teams para Mac

Para solucionar la falta de un complemento de Teams para los usuarios del sistema operativo Mac, siga estos pasos:

**Paso 1:** si tiene una implementación local de Exchange híbrida (2016 CU3 o posterior requerido), use la herramienta Test-HMA.ps1 para confirmar que la autenticación moderna híbrida está configurada correctamente. Para más información, consulte [Validar la configuración de la autenticación moderna híbrida para Outlook para iOS y Android](https://aka.ms/TestHMAEAS).  

**Nota:** utilice el formato de dirección UPN (por ejemplo, [username@contoso.com](mailto:username@contoso.com)), no el formato dominio\nombre de usuario. Haga esto incluso para los usuarios con buzones de Exchange Online.

**Paso 2:** haga que el usuario vaya a **Herramientas** > **Cuentas**... en Outlook para Mac y busque y seleccione la cuenta. Confirme que el nombre de usuario que aparece en la lista está en formato UPN (por ejemplo, [username@contoso.com](mailto:username@contoso.com)).

**Paso 3:** confirme que el usuario tiene licencia de Microsoft Teams. El usuario debe usar la suscripción a Office 365 para Mac, versión del producto 16.24 o posterior.