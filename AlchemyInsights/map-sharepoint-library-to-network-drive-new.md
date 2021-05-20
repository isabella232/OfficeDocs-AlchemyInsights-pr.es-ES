---
title: Asignar una biblioteca SharePoint a una unidad de red
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 6b7cb38362baa26bd39fe7478ef6dd1971b5b063
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52542838"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="086ca-102">Asignar una biblioteca SharePoint a una unidad de red</span><span class="sxs-lookup"><span data-stu-id="086ca-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="086ca-103">En lugar de asignar una unidad de red, SharePoint archivos con el nuevo cliente de sincronización OneDrive, que proporciona Archivos a petición.</span><span class="sxs-lookup"><span data-stu-id="086ca-103">Instead of mapping a network drive, sync SharePoint files with the new OneDrive sync client, which provides Files On-Demand.</span></span> <span data-ttu-id="086ca-104">Obtenga acceso a todos los archivos en OneDrive sin usar el espacio de almacenamiento local.</span><span class="sxs-lookup"><span data-stu-id="086ca-104">Access all your files in OneDrive without using local storage space.</span></span> <span data-ttu-id="086ca-105">Para obtener más información, vea [Sync SharePoint and Teams files with your computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) y Save disk space with OneDrive Files [On-Demand for Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="086ca-105">For more information, see [Sync SharePoint and Teams files with your computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) and [Save disk space with OneDrive Files On-Demand for Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span>

<span data-ttu-id="086ca-106">Si decide asignar una unidad en lugar de usar el nuevo cliente de [sincronización OneDrive,](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)asegúrese de seguir estos pasos:</span><span class="sxs-lookup"><span data-stu-id="086ca-106">If you choose to map a drive instead of using [the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88), make sure you follow these steps:</span></span>

- [<span data-ttu-id="086ca-107">Solucionar problemas de unidades de red asignadas que se conectan a SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="086ca-107">Troubleshoot mapped network drives that connect to SharePoint Online</span></span>](/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [<span data-ttu-id="086ca-108">Los errores de autenticación se producen cuando el cliente no tiene compatibilidad con TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="086ca-108">Authentication errors occur when client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

<span data-ttu-id="086ca-109">**NOTA:** Si usa Internet Explorer 10 con Windows 8 o Windows 7 y recibe Acceso  denegado  o Ruta de acceso no es accesible al asignar una unidad, resuelva este problema instalando esta [revisión](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d).</span><span class="sxs-lookup"><span data-stu-id="086ca-109">**NOTE:** If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, resolve this problem by installing this [hotfix](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d).</span></span>