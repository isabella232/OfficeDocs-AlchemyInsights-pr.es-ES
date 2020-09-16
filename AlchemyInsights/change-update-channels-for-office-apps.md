---
title: Cambiar los canales de actualización de las aplicaciones de Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 70b416e2b572fe9b4257648e3426b4d36975681e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756516"
---
# <a name="change-update-channels-for-office-apps"></a>Cambiar los canales de actualización de las aplicaciones de Office

Para las nuevas instalaciones de Office, use la configuración de descarga de software de Office para seleccionar el canal de actualización que prefiera y, a continuación, instale (o vuelva a instalar) las aplicaciones de Office. Para obtener más información, consulte [administrar la configuración de descarga de software en Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Tenga en cuenta** El canal de actualización seleccionado con la configuración de descarga de software de Office se aplica a todos los usuarios que realizan nuevas instalaciones mediante el portal de O365. Para obtener más información, consulte [Descargar e instalar o volver a instalar Microsoft 365 u Office 2019 en un equipo PC o Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Para las instalaciones existentes de Office, use la herramienta de implementación de Office (ODT) para cambiar a otro canal de actualización:  

1. Descargue la versión más reciente de la ODT (setup.exe) desde el [Centro de descarga de Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifique el nombre del canal al que quiere cambiar. Para obtener más información, consulte [Opciones de configuración para la Herramienta de implementación de Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Cree un archivo de configuración XML que especifique el nombre de canal apropiado, por ejemplo, Update. Xml.  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. Desde un símbolo del sistema con privilegios elevados, cambie a la ubicación de la carpeta donde se encuentra Setup. exe y ejecute el comando siguiente:  
    a. setup.exe /configure update.xml
5. Inicie una aplicación de Office (por ejemplo, Excel) y, a continuación, seleccione **Cuenta** > ** de archivo**. En la sección Información del producto, seleccione **Opciones de actualización** > **Actualizar ahora**.

Para obtener más información, consulte [Cómo cambiar los canales de actualización de las aplicaciones de Office existentes](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Para cambiar los canales de actualización de un grupo seleccionado de usuarios o mediante Configuration Manager (SCCM), configure la opción de configuración del canal de actualización con el GPO. Para más información, vea [Información general de los canales de actualización para Aplicaciones de Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Para obtener más información, consulte [Cómo administrar los canales de Office 365 ProPlus para profesionales de TI](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) y [Administrar las actualizaciones de Aplicaciones de Microsoft 365 con el Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).