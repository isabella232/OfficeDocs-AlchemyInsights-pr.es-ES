---
title: 932 Actualizar AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104829"
---
# <a name="upgrade-azure-ad-connect"></a>Actualizar Azure AD Conectar

De forma predeterminada, la actualización automática está habilitada para Azure AD Conectar, lo que ayuda a garantizar que ejecutes la versión más reciente. Para comprobar la configuración de actualización automática, use el cmdlet **Get-ADSyncAutoUpgrade** en PowerShell de Azure AD. El cmdlet devolverá uno de los siguientes valores:

- **Habilitado:** la actualización automática está habilitada.

- **Deshabilitado:** la actualización automática está deshabilitada.

- **Suspendido:** el sistema ya no es apto para recibir actualizaciones automáticas. No puede configurar este valor; lo establece el sistema.

Para obtener más información, vea [Actualización automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Para descargar la versión más reciente de Azure AD Conectar, vaya a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
