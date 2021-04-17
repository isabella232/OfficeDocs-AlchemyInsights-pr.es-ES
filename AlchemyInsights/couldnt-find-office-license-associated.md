---
title: Corregir aplicaciones de Microsoft 365 No se pudo encontrar el mensaje asociado a licencias de office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816505"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Corregir el mensaje de aplicaciones de Microsoft 365 "No se pudieron encontrar licencias de office asociadas"

Si recibe este mensaje, pruebe lo siguiente:

1. Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a las aplicaciones de Microsoft 365. Consulte Direcciones URL e intervalos de direcciones IP de [Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Quitar y [reasignar la licencia de Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para el usuario afectado. 
3. Abra una aplicación de Office y [salga de](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) cualquier cuenta de usuario existente.
4. Ve a Configuración de Windows > **Cuentas** de correo & cuentas y quita todas las cuentas de trabajo  >  excepto la cuenta afectada.
5. Ve a Configuración de Windows > **Acceso a** cuentas laborales o educativas y desconecta todas las cuentas de trabajo excepto la  >  cuenta afectada.
6. Restablezca el estado de activación de Office. [Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Inicie sesión](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.

Para obtener soluciones de solución de problemas adicionales, vea Errores de activación y productos sin [licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).