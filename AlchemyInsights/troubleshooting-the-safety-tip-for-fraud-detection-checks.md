---
title: Solución de problemas de consejo de seguridad de detección de fraudes
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955983"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Solución de problemas de consejo de seguridad de detección de fraudes

Si está obteniendo un consejo de seguridad que indica "El remitente ha fallado nuestras comprobaciones de detección de fraude y puede que no sea quien parece ser", el remitente no pudo pasar las comprobaciones de autenticación DKIM o SPF. El mejor método para resolver esto es que el remitente se autorice. Si el remitente envía en su nombre, debe autorizarlos agregando la dirección IP del remitente al registro SPF.
  
Consulta [Troubleshooting the red (suspicious) consejo de seguridad para ver comprobaciones de detección de fraudes](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obtener más información.
  
Estos son algunos otros vínculos que pueden ayudar:
  
- [Cómo Microsoft usa el marco de directivas de remitente (SPF) para evitar la suplantación de identidad](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar SPF para ayudar a evitar la suplantación de identidad](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
