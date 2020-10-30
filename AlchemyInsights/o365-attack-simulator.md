---
title: Simulador de ataque de 2681 en Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801568"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de ataques en Microsoft 365

- ¿Falta el simulador de ataque? El simulador **de ataque requiere Microsoft defender para Office 365 plan 2 (ATP plan 2)** u **Office 365 Enterprise E5** . El simulador de ataque **no** se incluye en Microsoft defender para Office 365 plan 1 (ATP plan 1), Office 365 Enterprise E3 ni ninguna de las suscripciones de Microsoft 365 apps for Business.

- La cuenta que use para iniciar ataques simulados requiere permisos de administrador global o de administrador de seguridad y autenticación multifactor (MFA). Para obtener más información acerca de los requisitos de los simuladores de ataques, vea [este tema](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Aspectos importantes que debe conocer sobre las simulaciones de ataque de **fuerza de contraseña** :

  - Si la cuenta de destino tiene MFA habilitado y la contraseña se ha adivinado correctamente, la cuenta no se mostrará como comprometida (el segundo factor de autenticación será incompleto).

  - El archivo de contraseña no puede tener más de 10 MB. Use una contraseña por línea e incluya una línea en blanco (retorno de carro) después de la última contraseña de la lista.

- Aspectos importantes que debe conocer sobre las simulaciones de conexión de **"Spear phishing"** :

  - Por diseño, no puede proporcionar un valor personalizado para la **dirección URL del servidor de inicio de sesión de suplantación de identidad** .

  - Si un destinatario usa el [complemento habilitar el mensaje de informe](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para informar del mensaje como suplantación de identidad (phishing), es posible que no reciba alertas del mensaje (ya que se trata de un ataque simulado).

- Informes: una vez completado el ataque simulado, puede hacer clic en detalles de los **ataques** para ver el informe.

- Para obtener instrucciones detalladas y nuevas características en el simulador de ataques, consulte [simulador de ataques en Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
