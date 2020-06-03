---
title: Código de error 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si recibe un error al activar Office 2013 en implementaciones de servicios de escritorio remoto (RDS), considere la posibilidad de habilitar ADAL editando el registro.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506863"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="f4971-103">Error al activar Office 2013 en servicios de escritorio remoto</span><span class="sxs-lookup"><span data-stu-id="f4971-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="f4971-104">Si recibe un error al activar Office 2013 en implementaciones de servicios de escritorio remoto (RDS), considere la posibilidad de habilitar ADAL editando el registro.</span><span class="sxs-lookup"><span data-stu-id="f4971-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="f4971-105">**Clave del registro**</span><span class="sxs-lookup"><span data-stu-id="f4971-105">**Registry key**</span></span>|<span data-ttu-id="f4971-106">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="f4971-106">**Type**</span></span>|<span data-ttu-id="f4971-107">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f4971-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f4971-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f4971-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f4971-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f4971-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f4971-110">1 </span><span class="sxs-lookup"><span data-stu-id="f4971-110">1</span></span>  <br/> |

<span data-ttu-id="f4971-111">Para obtener más información, consulte [Habilitar la autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f4971-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f4971-112">ADAL está habilitado de forma predeterminada en las aplicaciones de Microsoft 365 para empresas y Office 2016.</span><span class="sxs-lookup"><span data-stu-id="f4971-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="f4971-113">Servicios de escritorio remoto (RDS) se llamaba Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="f4971-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  