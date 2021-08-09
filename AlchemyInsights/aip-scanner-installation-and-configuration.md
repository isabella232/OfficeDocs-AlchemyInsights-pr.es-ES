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
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934274"
---
# <a name="aip-scanner-installation-and-configuration"></a>Escáner de AIP: Instalación y configuración

**Para instalar el escáner de AIP, siga las instrucciones recomendadas**:

1. Si está actualizando y no está realizando una instalación limpia, asegúrese de que ha seguido las instrucciones para la [actualización del escáner de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner); y, para el cliente de etiquetado unificado, consulte [actualización del escáner de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Compruebe que cumple con todos los [requisitos de configuración de firewall e infraestructura de red](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Asegúrese de que [las directivas estén configuradas](https://docs.microsoft.com/azure/information-protection/configure-policy) en etiquetado automático o que cuenten con una etiqueta predeterminada en la directiva.
4. Asegúrese de que el tipo de archivo relevante esté configurado para la etiqueta o la protección, tal y como se describe en [Tipos de archivo compatibles con el cliente de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Además, si quiere cambiar el comportamiento predeterminado, siga estas instrucciones: [Cambiar el nivel de protección predeterminado de los archivos](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Compruebe que la cuenta de usuario configurada para ejecutar el servicio de escáner tiene permisos de acceso a todos los repositorios configurados.
6. Si sigue experimentando problemas, exporte los registros del escáner y agréguelos al vale de soporte.

**Exportar los registros de escáner de Azure Information Protection**

1. Vaya a%localappdata%\Microsoft\MSIP en el contexto de usuario que ejecuta el servicio de análisis.
2. Comprima en un ZIP todo el contenido de la carpeta MSIP.
3. Guarde los registros en la ubicación que desee y adjúntelos a su solicitud de servicio.
4. También puede usar [Export-AIPLogs-Onbehalfof](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Para obtener más información, consulte:**
- [Implementación del escáner de Azure Information Protection para clasificar y proteger los archivos de forma automática](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Especificar y usar el parámetro token para Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Ejecutar un ciclo de detección y ver informes del escáner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Revisar la documentación de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisitos de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Descargar el cliente de Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
