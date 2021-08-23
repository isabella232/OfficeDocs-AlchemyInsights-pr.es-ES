---
title: Configuración Outlook etiqueta predeterminada no aplicada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370215"
---
# <a name="default-outlook-label-setting-not-applied"></a>Configuración Outlook etiqueta predeterminada no aplicada

Si la configuración de etiqueta predeterminada de Outlook no se aplica correctamente y se aplica una etiqueta diferente o ninguna etiqueta, podría experimentar un problema conocido (MC277818) y debe realizar una de estas 2 opciones para resolver el problema:

**Opción 1:**

1. Vaya a Microsoft 365 Centro de cumplimiento > **Soluciones de** protección de la  >  **información**.
1. Seleccione **Directivas de** etiqueta y seleccione la directiva de etiqueta que necesita editar ( La configuración de **OutlookDefaultlabel** no está establecida correctamente en la directiva de etiqueta en cuestión. Ejecute **Get-labelpolicy** para ver esta configuración y, a continuación, seleccione **Editar directiva**.
1. Seleccione **Siguiente** hasta que vea la configuración Aplicar esta etiqueta predeterminada a los correos **electrónicos,** que está disponible si selecciona Requerir que los usuarios apliquen una etiqueta **a** los correos electrónicos y documentos herederos en el cuadro **de** diálogo Configuración de directiva.
1. En el cuadro de diálogo Aplicar **una etiqueta predeterminada a documentos,** elija **Ninguno** en la lista desplegable.
1. Seleccione **Siguiente** y **Enviar para** guardar la configuración de la etiqueta.

**Opción 2:**

En [Powershell del](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Centro de seguridad y cumplimiento, use el comando Set-LabelPolicy para cambiar la etiqueta **OutlookDefault a** **Ninguno** en {OutlookDefaultLabel="None"}.

Ejecutar: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Para obtener más información sobre las etiquetas predeterminadas para Outlook, vea [Set a different default label for Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).