---
title: Controlar las actualizaciones automáticas de las aplicaciones de Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431792"
---
# <a name="control-automatic-updates-for-office-apps"></a>Controlar las actualizaciones automáticas de las aplicaciones de Office

De forma predeterminada, las actualizaciones de las aplicaciones de Office se descargan de forma automática y se aplican en segundo plano sin la intervención de usuarios o administradores. Sin embargo, los administradores pueden controlar cómo se aplican las actualizaciones en la configuración de Office Update. La configuración de actualizaciones permite a los administradores habilitar o deshabilitar las actualizaciones automáticas, mostrar u ocultar el botón **Actualizar ahora** en Office, establecer las fechas límite de las actualizaciones y mucho más. Para obtener información detallada, consulte:

- [Configuración de actualizaciones de Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Las actualizaciones automáticas de Office no están habilitadas](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definir el modo de actualización Office una vez instalado](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Para revisar la configuración de actualizaciones existente que se ha aplicado a un equipo cliente, siga estos pasos:

1. Abra el editor del registro en **Inicio** > **Ejecutar** > **regedit**.
2. Cambiar a la siguiente ubicación y revisar la configuración de Office Update:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Nota**  Si se establece la clave OfficeMgmtCOM, es posible que vea el mensaje "El administrador del sistema administra las actualizaciones" en **Office** > **Cuenta** > **Actualizaciones de Office**. Para obtener más información, consulte[Administrar actualizaciones de Aplicaciones de Microsoft 365 con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  