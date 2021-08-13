---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: c2f2a0c3888920a969a6fc70af7ef7bfd8435bdcf975e0f31452b5da85e3a208
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968898"
---
# <a name="blocking-legacy-authentication"></a>Bloqueo de la autenticación heredada

La autenticación heredada es un término que hace referencia a una solicitud de autenticación realizada por:

- Clientes Office que no usan la autenticación moderna (por ejemplo, Office cliente de 2010).

- Cualquier cliente que use protocolos de correo heredados como IMAP/SMTP/POP3.

Para obtener más información sobre cómo bloquear la autenticación heredada y habilitar la autenticación moderna, consulte [Bloqueo de la autenticación heredada.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Los valores predeterminados de seguridad Azure Active Directory (Azure AD) facilitan la seguridad y ayudan a proteger la organización. Los valores predeterminados de seguridad contienen opciones de seguridad preconfiguradas para ataques comunes.
Para obtener más información acerca de los valores predeterminados de seguridad, consulte [¿Cuáles son los valores predeterminados de seguridad?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Nota:** Si el espacio empresarial se creó el 22 de octubre de 2019 o después de él, es posible que experimente el nuevo comportamiento seguro de forma predeterminada y ya tenga los valores predeterminados de seguridad habilitados en el espacio empresarial.  In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.
