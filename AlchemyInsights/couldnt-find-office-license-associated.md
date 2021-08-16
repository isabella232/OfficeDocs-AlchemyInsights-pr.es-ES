---
title: Corregir Microsoft 365 aplicaciones no se pudo encontrar el mensaje asociado a licencias de office
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069621"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Corregir el mensaje Microsoft 365 aplicaciones de office "No se pudieron encontrar licencias de office asociadas"

Si recibe este mensaje, pruebe lo siguiente:

1. Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a Microsoft 365 aplicaciones. Vea [Microsoft 365 direcciones URL e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Quite y [vuelva a asignar Office licencia para](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) el usuario afectado. 
3. Abra un Aplicación de Office cerrar [sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de las cuentas de usuario existentes.
4. Vaya a Windows Configuración > **Cuentas de** correo & cuentas de correo electrónico y quite todas las cuentas  >  de trabajo excepto la cuenta afectada.
5. Vaya a Windows Configuración > **acceso a** cuentas laborales o educativas y desconecte todas las cuentas  >  de trabajo excepto la cuenta afectada.
6. Restablezca el estado de activación de Office. [Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Inicie sesión](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.

Para obtener soluciones de solución de problemas adicionales, vea Errores de activación y productos sin [licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).