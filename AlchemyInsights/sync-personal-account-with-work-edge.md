---
title: Permitir que un usuario sincronice una cuenta personal con la cuenta profesional en Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: 4c246fcc9ef0e3a79c3e68be491e3e7f5c6edb0b
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603284"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Permitir que un usuario sincronice una cuenta personal con la cuenta profesional en Microsoft Edge

Asegúrese de que cumple estos criterios:

- Enterprise State Roaming está habilitado en el Centro de administración de Azure Active Directory, que requiere una suscripción para Azure Active Directory Premium o Enterprise Mobility + Security (EMS). Para obtener más información, consulte [Habilitar Enterprise State Roaming en Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Se cumple uno o dos de los criterios siguientes:
    - El servicio Azure Information Protection está habilitado para su espacio empresarial. Para obtener más información, consulte [Activar la protección de Azure Rights Management desde el Centro de administración de Microsoft 365](/azure/information-protection/activate-office365).
    - La característica Azure Active Directory Enterprise State Roaming (ESR) está habilitada para cualquier usuario o inquilino. Para obtener más información, consulte [¿Qué es Enterprise State Roaming?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Si AIP y ESR están deshabilitados, un mensaje de error informará a los usuarios que la sincronización no está disponible para sus cuentas.
