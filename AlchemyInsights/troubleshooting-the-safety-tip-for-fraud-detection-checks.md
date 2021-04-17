---
title: Solución de problemas de la sugerencia de seguridad para comprobaciones de detección de fraudes
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834748"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Solución de problemas de la sugerencia de seguridad para comprobaciones de detección de fraudes

Si está recibiendo una sugerencia de seguridad que indica "El remitente ha fallado nuestras comprobaciones de detección de fraude y puede que no sea quien parece ser", el remitente no pudo pasar las comprobaciones de autenticación DKIM o SPF. El mejor método para resolver esto es que el remitente se autorice. Si el remitente envía en su nombre, debe autorizarlos agregando la dirección IP del remitente al registro SPF.
  
Consulta Solución de problemas de la sugerencia de seguridad [roja (sospechosa)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obtener más información sobre las comprobaciones de detección de fraudes.
  
Estos son algunos otros vínculos que pueden ayudar:
  
- [Cómo Microsoft usa el marco de directivas de remitente (SPF) para evitar la suplantación de identidad](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar SPF para ayudar a evitar la suplantación de identidad](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
