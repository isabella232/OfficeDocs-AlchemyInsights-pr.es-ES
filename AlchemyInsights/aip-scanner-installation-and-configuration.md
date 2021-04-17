---
title: 'Escáner de AIP: Instalación y configuración'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821680"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="39f13-102">Escáner de AIP: Instalación y configuración</span><span class="sxs-lookup"><span data-stu-id="39f13-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="39f13-103">**Para instalar el escáner de AIP, siga las instrucciones recomendadas**:</span><span class="sxs-lookup"><span data-stu-id="39f13-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="39f13-104">Si está actualizando y no está realizando una instalación limpia, asegúrese de que ha seguido las instrucciones para la [actualización del escáner de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner); y, para el cliente de etiquetado unificado, consulte [actualización del escáner de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="39f13-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="39f13-105">Compruebe que cumple con todos los [requisitos de configuración de firewall e infraestructura de red](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="39f13-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="39f13-106">Asegúrese de que [las directivas estén configuradas](https://docs.microsoft.com/azure/information-protection/configure-policy) en etiquetado automático o que cuenten con una etiqueta predeterminada en la directiva.</span><span class="sxs-lookup"><span data-stu-id="39f13-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="39f13-107">Asegúrese de que el tipo de archivo relevante esté configurado para la etiqueta o la protección, tal y como se describe en [Tipos de archivo compatibles con el cliente de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="39f13-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="39f13-108">Además, si quiere cambiar el comportamiento predeterminado, siga estas instrucciones: [Cambiar el nivel de protección predeterminado de los archivos](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="39f13-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="39f13-109">Compruebe que la cuenta de usuario configurada para ejecutar el servicio de escáner tiene permisos de acceso a todos los repositorios configurados.</span><span class="sxs-lookup"><span data-stu-id="39f13-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="39f13-110">Si sigue experimentando problemas, exporte los registros del escáner y agréguelos al vale de soporte.</span><span class="sxs-lookup"><span data-stu-id="39f13-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="39f13-111">**Exportar los registros de escáner de Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="39f13-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="39f13-112">Vaya a%localappdata%\Microsoft\MSIP en el contexto de usuario que ejecuta el servicio de análisis.</span><span class="sxs-lookup"><span data-stu-id="39f13-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="39f13-113">Comprima en un ZIP todo el contenido de la carpeta MSIP.</span><span class="sxs-lookup"><span data-stu-id="39f13-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="39f13-114">Guarde los registros en la ubicación que desee y adjúntelos a su solicitud de servicio.</span><span class="sxs-lookup"><span data-stu-id="39f13-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="39f13-115">También puede usar [Export-AIPLogs-Onbehalfof](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="39f13-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="39f13-116">**Para obtener más información, consulte:**</span><span class="sxs-lookup"><span data-stu-id="39f13-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="39f13-117">Implementación del escáner de Azure Information Protection para clasificar y proteger los archivos de forma automática</span><span class="sxs-lookup"><span data-stu-id="39f13-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="39f13-118">Especificar y usar el parámetro token para Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="39f13-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="39f13-119">Ejecutar un ciclo de detección y ver informes del escáner</span><span class="sxs-lookup"><span data-stu-id="39f13-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="39f13-120">Revisar la documentación de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="39f13-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- <span data-ttu-id="39f13-121">[Requisitos de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="39f13-121">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>
- [<span data-ttu-id="39f13-122">Descargar el cliente de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="39f13-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
