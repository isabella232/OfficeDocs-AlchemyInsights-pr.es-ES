---
title: 'Microsoft Teams: acceso de invitado'
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012325"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams: acceso de invitado

Si necesita ayuda para comunicarse con usuarios externos a su organización en Teams, debe decidir si desea usar el acceso de invitado o el acceso externo [(federación)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)o puede usar ambos.

Asegúrese de revisar [las diferencias para](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) comprender las características disponibles para cada una.  Por ejemplo, el acceso externo (federación) permite comunicaciones 1:1, como chat y presencia.  Sin embargo, los usuarios federados no pueden participar Teams colaboración.  Si quieres que un usuario externo se una y participe en conversaciones de canal de Teams o compartir archivos, tendrás que activar El acceso de invitado.

**Opción 1: Activar el acceso de invitado** En el Centro Teams administración, vaya a Org [Wide Configuración > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) y active "Permitir el acceso de invitado en Teams".  Para un inquilino con todas las demás configuraciones predeterminadas, esto debe ser todo lo que necesita hacer.  Para personalizar la configuración de Acceso de invitado, asegúrese de seguir todos los pasos de la lista de comprobación [de acceso de invitado](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Una vez que haya terminado completamente, tendrá que esperar hasta [24](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) horas para que la configuración suba a efecto.

Si estás seguro de que has completado todos los pasos de la lista de comprobación y han pasado más de 24 horas, sigue adelante e intenta agregar un invitado [a tu equipo](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Para obtener más información, incluidos los vídeos de cómo hacerlo, vea [Acceso de invitado en Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Opción 2: Activar el acceso externo (federación)** Si también desea activar el acceso externo (federación), en el Centro de administración de Teams vaya a Acceso externo de [Configuración >](https://admin.teams.microsoft.com/company-wide-settings/external-communications) para toda la organización y active "Los usuarios pueden comunicarse con usuarios de Skype Empresarial y Teams" y, a continuación, siga todos los pasos descritos en Permitir que los usuarios de Teams chatee y se comuniquen con usuarios de otra [organización.](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)
