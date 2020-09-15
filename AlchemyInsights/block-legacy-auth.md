---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685615"
---
# <a name="blocking-legacy-authentication"></a>Bloqueo de la autenticación heredada

La autenticación heredada es un término que hace referencia a una solicitud de autenticación realizada por:

- Clientes de Office antiguos que no usan la autenticación moderna (por ejemplo, Office 2010 Client).

- Cualquier cliente que use protocolos de correo heredados como IMAP/SMTP/POP3.

Para obtener más información sobre el bloqueo de la autenticación heredada y la habilitación de la autenticación moderna, consulte [blocking Legacy Authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).

Los valores predeterminados de seguridad en Azure Active Directory (Azure AD) hacen que sea más fácil ser seguro y ayudar a proteger su organización. Los valores predeterminados de seguridad contienen configuraciones de seguridad preconfiguradas para ataques comunes.
Para obtener más información acerca de los valores predeterminados de seguridad, consulte [¿Qué son los valores predeterminados de seguridad?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Nota**: Si el inquilino se creó el 22 de octubre de 2019, es posible que esté experimentando el nuevo comportamiento seguro de forma predeterminada y que ya tenga habilitada la seguridad predeterminada en su espacio empresarial.  En un esfuerzo por proteger a todos los usuarios, los valores predeterminados de seguridad se implementan en todos los nuevos inquilinos creados.
