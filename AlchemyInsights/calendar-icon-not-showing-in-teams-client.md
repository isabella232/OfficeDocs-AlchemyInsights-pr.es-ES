---
title: El icono de calendario no se muestra en el cliente de Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684715"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>El icono de calendario no se muestra en el cliente de Teams

La pestaña Calendario de Teams requiere el acceso a un buzón de Exchange a través de servicios Web de Exchange. El buzón de Exchange puede ser en línea o local. En el caso de los usuarios en línea que no vean la pestaña Calendario, asegúrese de que [tengan licencia para un buzón de Exchange Online y que el buzón esté habilitado](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Si el usuario tiene un buzón válido en Exchange Online pero aún no puede ver la pestaña Calendario, es posible que esté experimentando un problema de red. Use el [analizador de conectividad remota de Microsoft](https://testconnectivity.microsoft.com/) y ejecute las **pruebas de conectividad de servicios Web de Microsoft Exchange** para el usuario afectado.

Por último, compruebe las [directivas de configuración de aplicación para aplicaciones de Teams](https://admin.teams.microsoft.com/policies/app-setup) para asegurarse de que la aplicación de Calendario no se haya quitado de la directiva que se ha aplicado al usuario (lo más probable es que sea **Global (predeterminada para toda la organización)**.

Si sus usuarios están alojados en un entorno local, debe confirmar que la configuración híbrida es correcta. Use el [Asistente para la configuración híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar el problema.

Tenga en cuenta que [Teams requiere Exchange 2016 CU3 o una versión superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
