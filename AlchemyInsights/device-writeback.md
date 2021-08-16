---
title: Reescribición de dispositivos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101977"
---
# <a name="device-writeback"></a>Reescribición de dispositivos

La reescribición de dispositivos se usa en los siguientes escenarios:

- Habilitar [Windows Hello para empresas mediante la implementación híbrida de confianza de certificados](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Habilitar el acceso condicional basado en dispositivos a aplicaciones protegidas de ADFS (2012 R2 o superior) (confianzas de usuario de confianza de confianza)

    > [!NOTE]
    > Se requiere una suscripción Azure AD Premium para la reescripción del dispositivo.

Esto proporciona seguridad adicional y garantía de que el acceso a las aplicaciones solo se concede a dispositivos de confianza. Para obtener más información sobre el acceso condicional, vea [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) y Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).

Para obtener más información sobre habilitar la reescribición de dispositivos para dispositivos, consulta [Habilitar la reescribición de dispositivos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
