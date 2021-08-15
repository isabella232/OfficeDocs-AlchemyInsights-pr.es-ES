---
title: Falta correo electrónico en cuarentena
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
- "5668"
- "9002625"
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026239"
---
# <a name="missing-emails-in-quarantine"></a>Falta correo electrónico en cuarentena"

Los administradores [pueden ver, liberar o eliminar estos mensajes.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Para abrir el Centro de seguridad & cumplimiento, vaya a [https://protection.office.com](https://protection.office.com/) . Para abrir la página Cuarentena directamente, vaya a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puede buscar según los siguientes valores:  

- **Id. de mensaje**: El identificador único global del mensaje. Si selecciona un mensaje en la lista, el  valor **id.** de mensaje aparece en el panel desplegable Detalles que aparece. Los administradores pueden usar [seguimiento de mensajes](/microsoft-365/security/office-365-security/message-trace-scc) para buscar mensajes y los valores de Id. de mensaje correspondientes.
- **Dirección de correo electrónico del remitente**: Una única dirección de correo electrónico de remitente.
- **Dirección de correo electrónico del destinatario**: Una única dirección de correo electrónico de destinatario.
- **Asunto**: Use el asunto completo del mensaje. La búsqueda no distingue entre mayúsculas y minúsculas.

Cuando haya introducido los criterios de búsqueda, haga clic en ![Botón actualizar](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualizar** para filtrar los resultados.

Los cmdlets que usa para ver y administrar mensajes y archivos en cuarentena son:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)tenga en cuenta que este cmdlet solo es para mensajes, no archivos de malware de Microsoft Defender para Office 365 para SharePoint Online, OneDrive para la Empresa o Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)