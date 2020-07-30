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
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="01128-102">Controlar las actualizaciones automáticas de las aplicaciones de Office</span><span class="sxs-lookup"><span data-stu-id="01128-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="01128-103">De forma predeterminada, las actualizaciones de las aplicaciones de Office se descargan de forma automática y se aplican en segundo plano sin la intervención de usuarios o administradores.</span><span class="sxs-lookup"><span data-stu-id="01128-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="01128-104">Sin embargo, los administradores pueden controlar cómo se aplican las actualizaciones en la configuración de Office Update.</span><span class="sxs-lookup"><span data-stu-id="01128-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="01128-105">La configuración de actualizaciones permite a los administradores habilitar o deshabilitar las actualizaciones automáticas, mostrar u ocultar el botón **Actualizar ahora** en Office, establecer las fechas límite de las actualizaciones y mucho más.</span><span class="sxs-lookup"><span data-stu-id="01128-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="01128-106">Para obtener información detallada, consulte:</span><span class="sxs-lookup"><span data-stu-id="01128-106">For detailed information, see:</span></span>

- [<span data-ttu-id="01128-107">Configuración de actualizaciones de Office</span><span class="sxs-lookup"><span data-stu-id="01128-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="01128-108">Las actualizaciones automáticas de Office no están habilitadas</span><span class="sxs-lookup"><span data-stu-id="01128-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="01128-109">Definir el modo de actualización Office una vez instalado</span><span class="sxs-lookup"><span data-stu-id="01128-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="01128-110">Para revisar la configuración de actualizaciones existente que se ha aplicado a un equipo cliente, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="01128-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="01128-111">Abra el editor del registro en **Inicio** > **Ejecutar** > **regedit**.</span><span class="sxs-lookup"><span data-stu-id="01128-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="01128-112">Cambiar a la siguiente ubicación y revisar la configuración de Office Update:</span><span class="sxs-lookup"><span data-stu-id="01128-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="01128-113">a.</span><span class="sxs-lookup"><span data-stu-id="01128-113">a.</span></span> <span data-ttu-id="01128-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="01128-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="01128-115">b.</span><span class="sxs-lookup"><span data-stu-id="01128-115">b.</span></span> <span data-ttu-id="01128-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="01128-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="01128-117">**Nota**  Si se establece la clave OfficeMgmtCOM, es posible que vea el mensaje "El administrador del sistema administra las actualizaciones" en **Office** > **Cuenta** > **Actualizaciones de Office**.</span><span class="sxs-lookup"><span data-stu-id="01128-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="01128-118">Para obtener más información, consulte[Administrar actualizaciones de Aplicaciones de Microsoft 365 con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="01128-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  