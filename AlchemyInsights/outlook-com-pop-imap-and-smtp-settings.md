---
title: Configuración de POP, IMAP y SMTP para Outlook.com
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "780"
- "1415"
- "8000043"
ms.assetid: 16b5fbc6-6f45-4707-97bb-49a9b610ac56
ms.openlocfilehash: 1885297a578b433e5c74a4fc72557a1e0807cf40
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798177"
---
# <a name="pop-imap-and-smtp-settings-for-outlookcom"></a>Configuración de POP, IMAP y SMTP para Outlook.com

Si desea agregar su cuenta de Outlook.com a una aplicación de correo que admita POP o IMAP, esta es la configuración del servidor que necesitará:
  
- **Nombre del servidor IMAP:** Outlook.Office365.com
- **Puerto IMAP:** 993
- **Método de cifrado IMAP:** MTLS
- **Nombre del servidor POP:** Outlook.Office365.com  
- **Puerto pop:** 995  
- **Método de cifrado pop:** MTLS  
- **Nombre del servidor SMTP:** SMTP.Office365.com
- **Puerto SMTP:** 587
- **Método de cifrado SMTP:** STARTTLS

Obtenga más información sobre cómo [Agregar su cuenta de Outlook.com a otra aplicación de correo o Smart Device](https://support.office.com/article/73f3b178-0009-41ae-aab1-87b80fa94970?wt.mc_id=Office_Outlook_com_Alchemy).