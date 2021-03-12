---
title: Ejemplo de directiva contra suplantación de identidad de Microsoft Defender para Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737875"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Ejemplo de directiva contra suplantación de identidad de Microsoft Defender para Office 365

Estas opciones de configuración habilitan una directiva denominada *Dominio y CEO.* Esta directiva proporciona protección de usuario y dominio frente a la suplantación y, a continuación, aplica la directiva a todos los correos electrónicos recibidos por los usuarios del dominio. En primer lugar, agregue la siguiente información para crear la directiva:

- **Nombre:** Descripción del dominio y del director **general:** garantiza que el director ejecutivo y el dominio no se suplanten.
  **Se aplica a**: Select **El dominio de destinatario es**. En **Cualquiera de estos**, seleccione **Elegir** y, a continuación, seleccione un dominio. Seleccione **+ Agregar**. Active la casilla situada junto al nombre del dominio de la lista (por ejemplo, *contoso.com*) y, a continuación, **seleccione Agregar**. Seleccione **Listo**.
- Después de crear la directiva, puede ajustarla mediante las siguientes opciones:
  - **Agregar usuarios para proteger:** Para este ejemplo, agregue la dirección de correo electrónico del director general, como mínimo.
  - **Agregar dominios para proteger:** agregue el dominio organizativo que incluye la oficina del director general.
  - **Choose actions**: For **If email is sent by an suersonated user**, select Redirect message to another email **address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*). For **If email is sent by an suersonated domain**, select Quarantine the **message**.
  - **Inteligencia de buzones:** de forma predeterminada, esta opción se selecciona al crear una nueva directiva contra suplantación de identidad. Deje esta configuración **activada** para obtener mejores resultados.
  - **Agregar remitentes y dominios de confianza:** En este ejemplo, no defina ninguna invalidación.
- Una vez que hayas revisado la configuración, selecciona **Crear esta directiva** o **Guardar**, según corresponda.

Para obtener más información, vea [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
