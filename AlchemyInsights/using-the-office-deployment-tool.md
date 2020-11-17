---
title: Uso de la herramienta de implementación de Office
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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085849"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="d5896-102">Uso de la herramienta de implementación de Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="d5896-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d5896-103">Use la herramienta de implementación de Office (ODT) para implementar versiones de Office 365 de Office.</span><span class="sxs-lookup"><span data-stu-id="d5896-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="d5896-104">La herramienta de implementación de Office (setupodt.exe) se ejecuta desde la línea de comandos y usa un archivo de configuración XML para determinar qué configuración aplicar al implementar Office.</span><span class="sxs-lookup"><span data-stu-id="d5896-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="d5896-105">Descargue la versión más reciente de la herramienta de implementación de Office del [centro de descarga de Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="d5896-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="d5896-106">Use la [herramienta de personalización de Office (Oct)](https://config.office.com) para seleccionar sus preferencias de implementación y crear el archivo XML de configuración.</span><span class="sxs-lookup"><span data-stu-id="d5896-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="d5896-107">Exporte el archivo de configuración y colóquelo localmente en la misma carpeta en la que reside el setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="d5896-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="d5896-108">**Nota:** Los problemas de instalación de Office se producen normalmente debido a archivos de configuración mal configurados o con formato incorrecto.</span><span class="sxs-lookup"><span data-stu-id="d5896-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="d5896-109">Para evitar estos problemas, le recomendamos que use la herramienta de personalización de Office para crear el archivo de configuración.</span><span class="sxs-lookup"><span data-stu-id="d5896-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="d5896-110">También puede importar los archivos de configuración existentes en la herramienta de personalización de Office.</span><span class="sxs-lookup"><span data-stu-id="d5896-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="d5896-111">Desde un símbolo del sistema con privilegios elevados, cambie a la ubicación en la que reside setupodt.exe y ejecute la herramienta de implementación de Office en el modo de descarga y especifique el archivo de configuración que acaba de guardar.</span><span class="sxs-lookup"><span data-stu-id="d5896-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="d5896-112">En este ejemplo, el archivo de configuración se denomina Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="d5896-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="d5896-113">4. Ejecute la herramienta de implementación de Office en el modo de configuración y especifique el archivo de configuración.</span><span class="sxs-lookup"><span data-stu-id="d5896-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="d5896-114">**Nota:** Debe ejecutar este paso desde el equipo cliente en el que desea instalar Office y debe tener permisos de administrador local en ese equipo.</span><span class="sxs-lookup"><span data-stu-id="d5896-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="d5896-115">Para obtener más información sobre el uso de la herramienta de implementación de Office para los escenarios de implementación de aplicaciones de Microsoft 365 para empresas, vea [información general sobre la herramienta de implementación de Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="d5896-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="d5896-116">Para obtener más información sobre cómo usar la herramienta de personalización de Office, vea [información general sobre la herramienta de personalización de Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="d5896-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
