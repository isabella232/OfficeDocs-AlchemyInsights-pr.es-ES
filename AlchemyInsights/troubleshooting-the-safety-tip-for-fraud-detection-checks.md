---
title: Solución de problemas de la sugerencia de seguridad para las comprobaciones de detección de fraude
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658427"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Solución de problemas de la sugerencia de seguridad para las comprobaciones de detección de fraude

Si está recibiendo una sugerencia de seguridad que dice "el remitente produjo un error en nuestras comprobaciones de detección de fraude y puede no ser quien parece ser", entonces el remitente no ha podido pasar comprobaciones de autenticación DKIM o SPF. El mejor método para resolver esto es que el remitente autorice a sí mismo. Si el remitente está enviando en su nombre, debe autorizarlos agregando la dirección IP del remitente a su registro de SPF.
  
Consulte [solución de problemas de la sugerencia de seguridad en rojo (sospechoso) para las comprobaciones de detección de fraude](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obtener más información.
  
Estos son otros vínculos que pueden ayudarle:
  
- [Cómo usa Microsoft el marco de directivas de remitente (SPF) para evitar la suplantación de identidad](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar SPF para ayudar a evitar la suplantación de identidad](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
