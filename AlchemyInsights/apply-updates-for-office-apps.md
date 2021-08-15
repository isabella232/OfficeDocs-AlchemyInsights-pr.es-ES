---
title: Aplicar actualizaciones para aplicaciones de Office
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
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969402"
---
# <a name="apply-updates-for-office-apps"></a>Aplicar actualizaciones para aplicaciones de Office

De forma predeterminada, las actualizaciones de las aplicaciones de Office son gratuitas, descarga automáticamente y se aplican en segundo plano, sin la intervención del usuario. Para ejecutar las actualizaciones manualmente si tiene problemas para aplicar las actualizaciones, consulte [Instalar actualizaciones de Office](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5). Para obtener más información, consulte [Solucionar problemas de instalación de Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

Para administrar las actualizaciones de Office para los usuarios, tenga en cuenta estas opciones:

- Elija el canal de actualización de Office adecuado para su organización en función de la frecuencia de actualizaciones que desee. Para obtener más información, consulta [Información general de los canales de actualización para Aplicaciones de Microsoft 365](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).

- Decida si desea aplicar las actualizaciones automáticamente desde Internet o desde un recurso compartido local. Para obtener más información, consulte [Elegir cómo administrar las actualizaciones de las Aplicaciones de Microsoft 365](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).

- Revisar la configuración de Office Update para controlar cómo se aplican las actualizaciones en los equipos de los usuarios finales:

    - [Configure las opciones de actualización de las Aplicaciones de Microsoft 365](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [Define cómo se actualizará Office una vez instalado](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).

Cuando implemente aplicaciones de Office en varios usuarios, use la herramienta de personalización de Office para crear archivos de configuración para la implementación y configure las actualizaciones de Office con la herramienta de implementación de Office. Para obtener más información, consulte [Información general de la herramienta de personalización de Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) y la [Herramienta de implementación de Office](https://go.microsoft.com/fwlink/p/?LinkID=626065).

- Para ver un ejemplo de cómo configurar grupos de usuarios para implementar actualizaciones de Office, consulte [Implementar las Aplicaciones de Microsoft 365 desde un origen local](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).
-   Considere la posibilidad de usar la configuración ForceAppShutdown en caso de que las actualizaciones de Office no se apliquen a unos pocos usuarios por tener aplicaciones de Office abiertas. Para obtener más información, vea la [Propiedad de FORCEAPPSHUTDOWN (parte del elemento "Property")](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element). 

**Ver también**

[Información general sobre el proceso de actualización de las Aplicaciones de Microsoft 365](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Información de publicación de actualizaciones para las Aplicaciones de Microsoft 365](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)  
[Administrar las actualizaciones de Aplicaciones de Microsoft 365 con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).  
