---
title: Centro de administración de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049361"
---
# <a name="teams-admin-center"></a>Centro de administración de Teams

Obtenga información acerca de cómo administrar Teams con el [Centro de administración de Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Si no puede acceder al Centro de administración de Teams, compruebe los siguientes elementos:

- Compruebe que ha permitido las [direcciones IP y URL de Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) adecuadas en cualquier dispositivo perimetral (firewall, etc.) o en las reglas de firewall de su equipo local.
- Compruebe que el inicio de sesión que usa para obtener acceso al Portal de administración de Teams coincide con el nombre de usuario que indicó en el [Portal de administración de Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Si los usuarios no aparecen en el Centro de administración de Teams, consulte lo siguiente:

- ¿Ha creado usuarios o asignado licencias en las últimas 24 horas? Asegúrese de que espera al menos 24 horas antes de abrir un vale de soporte técnico.
- Compruebe que ha asignado las licencias adecuadas.
- Si tiene un directorio local de Active Directory, compruebe que [el valor de msRTCSIP-PrimaryUserAddress o la dirección SIP en el campo ProxyAddresses de su Active Directory local es único y el formato coincide con](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) la sip:**nombre de usuario** del usuario del [Centro de administración de Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Si tiene previsto mantener una implementación de Skype Empresarial Server y hacer que los usuarios estén alojados de manera local y en línea, siga la **"Configuración híbrida con Teams y Skype Empresarial Online"** en el panel de control de Skype Empresarial Server y mueva a los usuarios en línea.
