---
title: Configuración de POP, IMAP y SMTP en Outlook en la web
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
ms.openlocfilehash: a3f717754a5ebe5c73624553521241d57b38a7da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759200"
---
# <a name="pop-imap--smtp-settings-for-outlook-on-the-web"></a>Configuración de POP, IMAP & SMTP para Outlook en la web

Si desea agregar la cuenta de Microsoft 365 a otra aplicación de correo que admita POP, IMAP o SMTP, esta es la configuración manual del servidor que necesitará:
  
- **Nombre del servidor IMAP:** Outlook.Office365.com
- **Puerto IMAP:** 993
- **Método de cifrado IMAP:** SSL/TLS
- **Nombre del servidor POP:** Outlook.Office365.com  
- **Puerto pop:** 995  
- **Método de cifrado pop:** SSL/TLS  
- **Nombre del servidor SMTP:** SMTP.Office365.com
- **Puerto SMTP:** 587
- **Método de cifrado SMTP:** STARTTLS