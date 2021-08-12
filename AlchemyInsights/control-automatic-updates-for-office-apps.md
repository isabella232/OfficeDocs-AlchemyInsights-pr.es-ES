---
title: Controlar las actualizaciones automáticas de las aplicaciones de Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929898"
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