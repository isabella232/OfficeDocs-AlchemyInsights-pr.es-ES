---
title: Sincronización de hash de contraseña para el servicio de dominio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040883"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sincronización de hash de contraseña para el servicio de dominio

**Si su instancia de Azure AD DS le pide que habilite la sincronización de hash de contraseña**

Se encuentra con un escenario en el que está ejecutando un entorno híbrido con usuarios que realizan sincronizaciones desde un entorno local de Azure Active Directory Domain Services (AD DS). Esto se da a pesar de que tiene configurada la sincronización de hash de contraseña desde la instancia de AD DS local con su inquilino de Azure AD.

**Causa**

Esto sucede porque Azure AD Connect no sincroniza de forma predeterminada los hashes de Kerberos y New Technology LAN Manager (NTLM) heredados que son necesarios para Azure AD DS.

**Solución alternativa** 

Necesitará configurar Azure AD Connect para sincronizar los hashes de contraseña necesarios para la autenticación NTLM y Kerberos.

Después de configurar Azure AD Connect, un evento de cambio de contraseña o de creación de cuenta local también sincroniza los hashes de contraseña heredados con Azure AD. Haga clic [aquí](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) para obtener más información sobre esto, así como instrucciones sobre cómo habilitar la sincronización de contraseñas en entornos híbridos de Azure AD DS.