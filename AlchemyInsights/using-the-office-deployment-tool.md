---
title: Uso de la Office de implementación
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083787"
---
# <a name="using-the-office-deployment-tool-odt"></a>Uso de la Office de implementación (ODT)

Use la herramienta Office implementación (ODT) para implementar Office 365 versiones de Office. La herramienta Office implementación (setup.exe) se ejecuta desde la línea de comandos y usa un archivo XML de configuración para determinar qué configuración se debe aplicar al implementar Office.
  
1. Descargue la versión más reciente de la herramienta Office implementación desde el [Centro de descarga de Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Use la [herramienta Office personalización (OCT)](https://config.office.com) para seleccionar las preferencias de implementación y crear el archivo XML de configuración. Exporte el archivo de configuración y colóculo localmente en la misma carpeta en la que setup.exe reside.

    **Nota:** Office de instalación normalmente se producen debido a archivos de configuración mal configurados o mal formatados. Para evitar estos problemas, se recomienda usar la herramienta de personalización Office para crear el archivo de configuración. También puede importar archivos de configuración existentes en la herramienta Office personalización.

3. Desde un símbolo del sistema con privilegios elevados, cambie a la ubicación donde reside setup.exe y ejecute la herramienta de implementación de Office en modo de descarga y especifique el archivo de configuración que acaba de guardar. En este ejemplo, el archivo de configuración se denomina Configuration.xml:

```setup.exe /download Configuration.xml```

4.Ejecute la herramienta Office implementación en modo de configuración y especifique el archivo de configuración.

```setup.exe /configure Configuration.xml```

**Nota:** Debe ejecutar este paso desde el equipo cliente en el que desea instalar Office y debe tener permisos de administrador local en ese equipo.

Para obtener más información sobre Office Deployment Tool para los escenarios Aplicaciones Microsoft 365 para empresas implementación, vea [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Para obtener más información sobre cómo usar la herramienta de personalización Office, vea [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
