---
title: Configuración de POP, IMAP y SMTP en Outlook en la Web
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: ''
ms.openlocfilehash: 2932a7cf3c6681e00455f8292716b46d911010a4d2c84d519f90b2ffa971b35f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960996"
---
# <a name="pop-imap--smtp-settings-for-outlook-on-the-web"></a>Pop, IMAP & smtp para Outlook en la Web

Si quieres agregar tu cuenta de Microsoft 365 a otra aplicación de correo que admita POP, IMAP o SMTP, esta es la configuración manual del servidor que necesitarás:
  
- **Nombre del servidor IMAP:** outlook.office365.com
- **Puerto IMAP:** 993
- **Método de cifrado IMAP:** SSL/TLS
- **Nombre del servidor POP:** outlook.office365.com  
- **Puerto POP:** 995  
- **Método de cifrado POP:** SSL/TLS  
- **Nombre del servidor SMTP:** smtp.office365.com
- **Puerto SMTP:** 587
- **Método de cifrado SMTP:** STARTTLS