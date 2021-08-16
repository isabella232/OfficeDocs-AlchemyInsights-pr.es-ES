---
title: 2681 Attack Simulator en Microsoft 365
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
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065301"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulador de ataque en Microsoft 365

- ¿Falta el simulador de ataque? Attack Simulator requiere **Microsoft Defender para Office 365 plan 2** o Office 365 Enterprise **E5**. Attack Simulator no **se incluye** en Microsoft Defender para Office 365 plan 1, Office 365 Enterprise E3 ni ninguna Aplicaciones Microsoft 365 para negocios suscripciones.

- La cuenta que use para iniciar ataques simulados requiere permisos de administrador global o de administrador de seguridad y autenticación multifactor (MFA). Para obtener más información acerca de los requisitos de Attack Simulator, vea [este tema](/microsoft-365/security/office-365-security/attack-simulator).

- Aspectos importantes que debe saber acerca de las simulaciones **de ataque** de contraseña de fuerza bruta:

  - Si la cuenta de destino tiene MFA habilitada y la contraseña se ha adivinado correctamente, la cuenta no se mostrará como comprometida (el segundo factor de autenticación estará incompleto).

  - El archivo de contraseña no puede tener más de 10 MB. Use una contraseña por línea e incluya una línea en blanco (retorno de carro) después de la última contraseña de la lista.

- Aspectos importantes que debe saber acerca de las simulaciones **de conexión de phishing** de Lanza:

  - Por diseño, no puede proporcionar un valor personalizado para la dirección URL del servidor de inicio de **sesión de phishing**.

  - Si un destinatario [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) usa el complemento Habilitar el mensaje de informe para notificar el mensaje como suplantación de identidad, es posible que no reciba alertas para el mensaje (porque se trata de un ataque simulado).

- Informes: una vez completado el ataque simulado, puedes hacer clic en **Detalles de ataque** para ver el informe.

- Para obtener instrucciones detalladas y nuevas características en Attack Simulator, consulta [Attack Simulator en Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
